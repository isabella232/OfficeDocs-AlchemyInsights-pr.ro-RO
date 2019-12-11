---
title: Implementarea Office 365 ProPlus pentru utilizarea partajată pe RDS, Terminal Server sau VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959471"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementarea Office 365 ProPlus pentru utilizarea partajată pe RDS, Terminal Server sau VDI

Pentru a implementa Office 365 ProPlus utilizând consolidare servicii Desktop la distanță (RDS), denumit anterior Terminal Services:
- Trebuie să aveți un Microsoft 365 pentru plan de afaceri sau un plan de Office 365 care include Office 365 ProPlus, ar fi Office 365 Enterprise E3 sau Enterprise E5.
   > [!NOTE] 
   > Planurile Office 365 Business și Office 365 Business Premium nu includ Office 365 ProPlus.
- Trebuie să activați [activarea computerului partajat](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> De asemenea, aveți posibilitatea să descărcați și să executați [Asistentul Microsoft pentru asistență și recuperare](https://aka.ms/SaRA_OfficeSCA_M365Portal) pentru a instala Office 365 ProPlus în modul de activare a computerului partajat.

Pentru mai multe informații despre cerințe preliminare, instrucțiuni de instalare și îndrumare pe instalări particularizate utilizând instrumentul de implementare Office, consultați [implementarea office 365 ProPlus utilizând consolidare servicii Desktop la distanță](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Pentru a remedia erorile legate de activarea computerului partajat:
- Consultați [Depanarea problemelor cu activarea computerului partajat pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Consultați [reinițializați starea de activare Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

Dacă doriți să instalați Office 365 ProPlus pe RDS de la centrul de administrare Microsoft 365, ***care utilizează setările de instalare implicite***, utilizați următorii pași:

1.  Verificați ce Office 365 plan aveți. [Invata](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Dacă este necesar, comutați la un alt plan Office 365. [Invata](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Dacă Office este deja instalat pe serverul RDS utilizând orice alte planuri de Office 365, dezinstalați-l. De exemplu, mergând la **panoul** > de control**Dezinstalați un program**. Dezinstalați utilizând [asistența Microsoft și asistentul de recuperare](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă executați probleme.
4.  Pe serverul RDS, conectați-vă la centrul de administrare Microsoft 365 cu contul de administrator și [Instalați Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  După ce Office este instalat, ***nu deschideți sau faceți sign in*** la orice aplicații Office.
6.  Pe serverul RDS, activați activarea computerului partajat editând registry urmând acești pași:
   1. Faceți clic dreapta pe butonul Windows din colțul din stânga jos al ecranului și selectați **Executare**. În caseta Deschidere, tastați **regedit**, apoi selectați **OK**.
   2. Selectați **Da** când vi se solicită să permiteți editorului de registry să facă modificări pe dispozitiv.
   3. În editorul de registry, adăugați o valoare șir de **Sharedcomputerlicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Pe serverul RDS, ***Conectați-vă ca utilizator final*** și [Verificați că activarea computerului partajat este activată pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

