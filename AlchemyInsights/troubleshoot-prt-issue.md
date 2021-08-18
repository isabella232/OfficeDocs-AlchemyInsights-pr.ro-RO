---
title: Depanarea problemei cu PRT
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
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330971"
---
# <a name="troubleshoot-prt-issue"></a>Depanarea problemei cu PRT

Pentru ca orice dispozitiv să se autentifice, acesta trebuie să fie înregistrat în întregime și în stare bună și să poată obține un token de reîmprospătare primară (PRT).

Procesul de înregistrare de asociere hibridă la Azure AD necesită ca dispozitivele să fie într-o rețea de corporație. De asemenea, funcționează prin VPN, dar există câteva avertismente în acest lucru. Am auzit clienții care au nevoie de asistență pentru depanarea procesului hibrid de înregistrare pentru asocierea Azure AD în situații de lucru la distanță. Iată o defalcare a ceea ce se întâmplă în cu totul în timpul procesului de înregistrare.

**Mediul de autentificare în cloud (utilizând sincronizarea hash-ului parolei Azure AD sau autentificarea "pass-through")**

Acest flux de înregistrare se mai știe și ca "Sincronizare asociere".

1. Windows 10 descoperi o înregistrare SCP la conectarea utilizatorului la dispozitiv.
    1. Dispozitivul încearcă mai întâi să regăsească informațiile entității găzduite din SCP pe partea client în registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pentru mai multe informații, consultați acest [document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Dacă nu reușește, dispozitivul comunică cu Active Directory local (AD) pentru a obține informații despre entitatea găzduită de la Punctul de conexiune serviciu (SCP). Pentru a verifica SCP, consultați acest [document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Notă:** Vă recomandăm să activați SCP în AD și să utilizați doar SCP pe partea client pentru validare inițială.

2. Windows 10 încearcă să comunice cu Azure AD în contextul de sistem pentru a se autentifica în Azure AD. Puteți verifica dacă dispozitivul poate accesa resurse Microsoft de sub contul de sistem, utilizând scriptul Test Device Registration Connectivity.

3. Windows 10 generează un certificat auto-semnat și îl stochează sub obiectul computer în AD local. Aceasta necesită linii de vedere către controlerul de domeniu.

4. Un obiect de dispozitiv care are un certificat este sincronizat cu Azure AD prin azure AD Conectare. Ciclul de sincronizare este o dată la fiecare 30 de minute în mod implicit, dar depinde de configurația Azure AD Conectare. Pentru mai multe informații, consultați acest [document.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. În această etapă ar trebui să vedeți dispozitivul subiect în starea "În așteptare" sub Blade dispozitiv al portalului Azure.

6. La următorul utilizator care se conectează la Windows 10, înregistrarea va fi finalizată. 

**Notă:** dacă vă a numărați prin VPN și un proces de conectare la logoff închide conexiunea la domeniu, puteți declanșa manual înregistrarea:
 1. Emiteți o dsregcmd /join local la solicitarea administratorului sau de la distanță prin PSExec pe PC. De exemplu, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Pentru mai multe detalii despre problemele de asociere hibridă, consultați [Depanarea problemelor cu dispozitivele.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
