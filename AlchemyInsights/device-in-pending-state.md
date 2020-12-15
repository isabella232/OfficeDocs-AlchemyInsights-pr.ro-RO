---
title: Dispozitiv în stare în așteptare
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679989"
---
# <a name="device-in-pending-state"></a>Dispozitiv în stare în așteptare

**Cerințe preliminare**

1. Dacă configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit [Introducere în gestionarea dispozitivelor în Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) care vă va ghida despre cum să obțineți dispozitive sub controlul Azure AD.
2. Dacă înregistrați dispozitivele în Azure AD direct și le înscrieți în Intune, va trebui să vă asigurați că ați [configurat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) și că [licența](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) a fost implementată mai întâi.
3. Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD și AD local. Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor. În plus, dacă configurați înregistrări automate în Active Directory local, va trebui să fiți administrator al Active Directory și AD FS (dacă este cazul).

Procesul de înregistrare a asocierii hibride Azure AD necesită ca dispozitivele să fie în rețeaua corporativă. De asemenea, funcționează prin VPN, dar există câteva limitări pentru aceasta. Am auzit clienți care au nevoie de asistență pentru depanarea procesului de înregistrare hibrid Azure AD Join-up, sub circumstanțe de lucru la distanță.

**Mediu de autentificare în cloud (utilizând Azure AD password hash-sincronizare sau autentificare directă)**

Acest flux de înregistrare este, de asemenea, cunoscut sub numele de "asociere la sincronizare".

Iată o defalcare a ceea ce se întâmplă în timpul procesului de înregistrare:

1. Windows 10 descoperă înregistrarea punctului de conexiune la serviciu (SCP) atunci când utilizatorul se conectează la dispozitiv.

    1. Dispozitivul încearcă mai întâi să regăsească informațiile despre entitatea găzduită din partea client SCP în registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pentru mai multe informații, consultați [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Dacă nu reușește, dispozitivul comunică cu Active Directory local pentru a obține informații despre entitatea găzduită de la SCP. Pentru a verifica SCP, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Vă recomandăm să activați SCP în Active Directory și doar să utilizați SCP client-side pentru validare inițială.

2. Windows 10 încearcă să comunice cu Azure AD sub contextul sistemului, pentru a se autentifica împotriva Azure AD.

    Puteți verifica dacă dispozitivul poate accesa resursele Microsoft sub contul sistemului, utilizând [scriptul de conectivitate pentru înregistrarea dispozitivelor de testare](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 generează certificat cu semnătură automată și îl stochează sub obiectul computer în Active Directory local. Acest lucru necesită o linie de vedere la controlerul de domeniu.

4. Obiectul dispozitiv care are certificat este sincronizat cu Azure AD prin Azure AD Connect. Ciclul de sincronizare este la fiecare 30 de minute în mod implicit, dar depinde de configurarea Azure AD Connect. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. În această etapă, ar trebui să puteți vedea dispozitivul subiect în starea "în **așteptare**" sub Blade Device din Azure portal.

6. La următorul utilizator de conectare la Windows 10, înregistrarea va fi finalizată.

    > [!NOTE]
    > Dacă vă aflați pe VPN și logoff/login termină conectivitatea domeniului, puteți să declanșați manual înregistrarea. Pentru a face acest lucru:
    >
    > Emiteți o `dsregcmd /join` Solicitare locală în administrare sau la distanță prin PSExec pe PC.
    >
    > De exemplu: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Pentru probleme comune cu înregistrarea dispozitivelor Azure Active Directory, consultați [întrebări frecvente despre dispozitive](https://docs.microsoft.com/azure/active-directory/devices/faq).
