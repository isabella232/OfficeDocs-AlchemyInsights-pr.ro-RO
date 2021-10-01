---
title: Implementarea Aplicații Microsoft 365 pentru întreprindere pentru utilizare partajată pe RDS, Terminal Server sau VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041018"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementarea Aplicații Microsoft 365 pentru întreprindere pentru utilizare partajată pe RDS, Terminal Server sau VDI

Pentru a Aplicații Microsoft 365 servicii desktop la distanță (RDS), anterior Terminal Services, trebuie să:

- Utilizați remedierea simplă pentru a activa TLS 1.2 ca implicit dacă rulați o versiune mai veche de Windows (de exemplu, Windows 7 SP1, Windows Server 2008 R2). Pentru remediere simplă și mai multe informații, consultați Actualizare pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)protocoale sigure implicite în WinHTTP în Windows . 
- Să aveți un plan care include Aplicații Microsoft 365 pentru întreprindere (anterior Office 365 Plus). De exemplu, Office 365 E3, Microsoft 365 E5 sau orice plan care include versiunea desktop de Project sau Visio, cum ar fi Project Plan 3 sau Visio Plan 2, sau planul Microsoft 365 Business Premium, care include și Aplicații Microsoft 365 pentru afaceri.
- Activați activarea computerului partajat. Pentru mai multe informații, consultați [Prezentare generală a activării computerului partajat pentru Aplicații Microsoft 365](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Notă:** Pentru a instala Aplicații Microsoft 365 în modul de activare a computerului partajat, descărcați și rulați [Microsoft Asistent pentru recuperare și asistență](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Pentru detalii despre cerințele preliminare, instrucțiunile de configurare și instrucțiunile pentru particularizarea instalărilor utilizând Instrumentul de implementare Office, consultați Implementarea Aplicații Microsoft 365 utilizând Servicii desktop la [distanță.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Pentru a remedia erorile legate de activarea computerului partajat, consultați:

- [Depanarea problemelor cu activarea computerului partajat pentru Aplicații Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Reinițializarea Aplicații Microsoft 365 pentru întreprindere de activare](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Dacă doriți să instalați RDS Aplicații Microsoft 365 pe RDS de pe Centru de administrare Microsoft 365, care utilizează setările de instalare implicite, urmați acești pași:

1. Verificați ce Microsoft 365 plan aveți. Pentru mai multe informații, [consultați Ce abonament am?.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

1. Dacă este necesar, comutați la alt Microsoft 365 plan. Pentru mai multe informații, consultați [Upgrade-ul la un alt plan.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Dacă Aplicații Microsoft 365 este deja instalat pe serverul RDS utilizând orice alte planuri incompatibile, dezinstalați-l accesând Dezinstalarea unui program din Panoul  >  **de control.** Dacă aveți probleme, dezinstalați prin descărcarea [Microsoft Asistent pentru recuperare și asistență](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. Pe serverul RDS, conectați-vă la Centru de administrare Microsoft 365 cu contul de administrator și [instalați Office](https://portal.office.com/OLS/MySoftware.aspx).

   După Office este instalat, nu deschideți aplicațiile și nu vă conectați la Office sistem.

1. Pe serverul RDS, activați activarea computerului partajat prin editarea registry:

   1. Faceți clic dreapta pe Windows din colțul din stânga jos al ecranului și selectați **Rulare**. În caseta Deschidere, tastați **regedit**, apoi selectați **OK**.

   1. Când vi se solicită să permiteți editorului de registry să facă modificări la dispozitivul dvs., selectați **Da.**

   1. În Registry Editor, sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, adăugați o valoare șir de caractere **SharedComputerLicensing** cu setarea **1** .

1. Pe serverul RDS, conectați-vă ca utilizator final și verificați dacă activarea computerului partajat este activată pentru Aplicații Microsoft 365. 

   Pentru detalii, consultați [Verificați dacă activarea computerului partajat este activată pentru Aplicații Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).