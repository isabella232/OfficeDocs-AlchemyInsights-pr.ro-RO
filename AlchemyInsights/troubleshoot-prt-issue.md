---
title: Depanarea problemei PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573724"
---
# <a name="troubleshoot-prt-issue"></a>Depanarea problemei PRT

Pentru ca orice dispozitiv să termine să se autentifice, acesta trebuie să fie înregistrat complet și în stare bună și să poată obține un token de reîmprospătare principală (PRT).

Procesul de înregistrare a asocierii hibride Azure AD necesită ca dispozitivele să fie într-o rețea corporativă. De asemenea, funcționează prin VPN, dar există câteva limitări pentru aceasta. Am auzit clienți care au nevoie de asistență cu depanarea procesului de înregistrare hibrid Azure AD Join-up în circumstanțe de la locul de muncă. Iată o defalcare a ceea ce se întâmplă "sub capota" în timpul procesului de înregistrare.

**Mediu de autentificare în cloud (utilizând Azure AD password hash-sincronizare sau autentificare directă)**

Acest flux de înregistrare este, de asemenea, cunoscut sub numele de "asociere la sincronizare".

1. Windows 10 descoperă o înregistrare SCP la conectarea la utilizator a dispozitivului.
    1. Dispozitivul încearcă mai întâi să regăsească informațiile despre entitatea găzduită din partea client SCP în registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Dacă nu reușește, dispozitivul comunică cu Active Directory local (AD) pentru a obține informații despre entitatea găzduită de la punctul de conexiune la serviciu (SCP). Pentru a verifica SCP, vă rugăm să consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Vă recomandăm să activați SCP în reclamă și să utilizați doar clientul-Side SCP pentru validare inițială.

2. Windows 10 încearcă să comunice cu Azure AD sub contextul sistemului, pentru a se autentifica împotriva Azure AD. Puteți verifica dacă dispozitivul poate accesa resursele Microsoft sub contul sistemului, utilizând scriptul de conectivitate pentru înregistrarea dispozitivelor de testare.

3. Windows 10 generează un certificat cu semnătură automată și îl stochează sub obiectul computer din reclama locală. Acest lucru necesită o linie de vedere la controlerul de domeniu.

4. Un obiect dispozitiv care are un certificat este sincronizat cu Azure AD prin Azure AD Connect. Ciclul de sincronizare este la fiecare 30 de minute în mod implicit, dar depinde de configurarea Azure AD Connect. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. În această etapă, ar trebui să puteți vedea dispozitivul subiect în starea "în așteptare" sub Blade Device din Azure portal.

6. La următorul utilizator de conectare la Windows 10, înregistrarea va fi finalizată. 

> [!NOTE]
> Dacă vă deconectați de la VPN și un proces de conectare la logoff termină conectivitatea domeniului, puteți să declanșați manual înregistrarea:
 1. Emiteți un dsregcmd/Join local pe un prompt de administrator sau la distanță prin PSExec pe PC. De exemplu, PsExec-s \\ win10client01 cmd, dsregcmd/Join

 2. Pentru mai multe detalii despre problemele de asociere hibrid, consultați [Depanarea problemei dispozitivelor](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
