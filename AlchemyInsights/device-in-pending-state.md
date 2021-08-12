---
title: Dispozitiv în stare de așteptare
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914015"
---
# <a name="device-in-pending-state"></a>Dispozitiv în stare de așteptare

**Cerințe preliminare:**

1. În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit Introducere în gestionarea dispozitivelor în [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) care vă va ghida despre cum să controlați Azure AD pentru dispozitive.
2. Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, va trebui să [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) vă asigurați că ați configurat [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) și că licențierea a fost configurată mai întâi.
3. Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD și AD local. Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor. În plus, în cazul în care configurați înregistrările automate în Active Directory local, va trebui să fiți administrator Active Directory și AD FS (dacă este cazul).

Procesul hibrid de înregistrare de asociere la Azure AD necesită ca dispozitivele să fie în rețeaua de corporație. De asemenea, funcționează prin VPN, dar există câteva avertismente în acest lucru. Am auzit clienții care au nevoie de asistență pentru depanarea procesului hibrid de înregistrare a unirii Azure AD în situații de lucru la distanță.

**Mediul de autentificare în cloud (utilizând sincronizarea hash-ului parolei Azure AD sau autentificarea "pass-through")**

Acest flux de înregistrare se mai știe și ca "Sincronizare asociere".

Iată o defalcare a ceea ce se întâmplă în timpul procesului de înregistrare:

1. Windows 10 descoperă înregistrarea Punct de conexiune serviciu (SCP) atunci când utilizatorul se conectează la dispozitiv.

    1. Dispozitivul încearcă mai întâi să regăsească informațiile entității găzduite din SCP pe partea client în registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Pentru mai multe informații, consultați [documentul.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Dacă nu reușește, dispozitivul comunică cu Active Directory local pentru a obține informații despre entitatea găzduită de la SCP. Pentru a verifica SCP, consultați acest [document.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Vă recomandăm să activați SCP în Active Directory și să utilizați doar SCP pe partea client pentru validare inițială.

2. Windows 10 încearcă să comunice cu Azure AD în contextul de sistem pentru a se autentifica în Azure AD.

    Puteți verifica dacă dispozitivul poate accesa resursele Microsoft din contul de sistem, utilizând [scriptul Test Device Registration Connectivity.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 generează certificat auto-semnat și îl stochează sub obiectul computer din Active Directory local. Aceasta necesită linii de vedere către controlerul de domeniu.

4. Obiectul de dispozitiv care are certificat este sincronizat cu Azure AD prin azure AD Conectare. Ciclul de sincronizare este o dată la fiecare 30 de minute în mod implicit, dar depinde de configurația Azure AD Conectare. Pentru mai multe informații, consultați acest [document.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. În această etapă ar trebui să vedeți dispozitivul subiect în **starea**" În așteptare " sub Device blade of Azure Portal.

6. La următorul utilizator care se conectează la Windows 10, înregistrarea va fi finalizată.

    > [!NOTE]
    > Dacă sunteți la VPN și conectare/conectare se închide conexiunea la domeniu, puteți declanșa manual înregistrarea. Pentru aceasta:
    >
    > Emiteți `dsregcmd /join` o solicitare locală de administrare sau la distanță prin PSExec pe PC.
    >
    > De exemplu: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Pentru probleme comune cu înregistrarea Azure Active Directory, consultați Întrebări frecvente [despre dispozitive.](https://docs.microsoft.com/azure/active-directory/devices/faq)
