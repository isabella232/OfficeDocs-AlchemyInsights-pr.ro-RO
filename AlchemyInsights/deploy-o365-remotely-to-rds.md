---
title: Implementarea Aplicațiilor Microsoft 365 pentru întreprindere pentru utilizare partajată pe RDS, Terminal Server sau VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704717"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementarea Aplicațiilor Microsoft 365 pentru întreprindere pentru utilizare partajată pe RDS, Terminal Server sau VDI

Pentru a implementa Microsoft 365 Apps for enterprise utilizând Remote Desktop Services (RDS), denumit anterior Terminal Services:
- Trebuie să aveți un plan Microsoft 365 pentru firme sau un plan Office 365 care include Microsoft 365 Apps for enterprise, ar fi Office 365 Enterprise E3 sau Enterprise E5.
   > [!NOTE] 
   > Planurile Microsoft 365 Apps for business și Microsoft 365 Business Premium Standard nu includ Microsoft 365 Apps for enterprise.
- Trebuie să activați [activarea computerului partajat](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> De asemenea, puteți descărca și executa [Asistentul de asistență și recuperare Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pentru a instala Microsoft 365 Apps for enterprise în modul de activare a computerului partajat.

Pentru mai multe informații despre cerințe preliminare, instrucțiuni de instalare și indicații privind instalările particularizate utilizând Instrumentul de implementare Office, consultați [Implementarea aplicațiilor Microsoft 365 pentru întreprinderi utilizând Serviciile Desktop la distanță](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Pentru a remedia erorile legate de activarea computerului partajat:
- Consultați [Depanarea problemelor cu activarea computerului partajat pentru Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Consultați [Resetarea aplicațiilor Microsoft 365 pentru starea de activare pentru întreprinderi](https://go.microsoft.com/fwlink/?linkid=2109218).

Dacă doriți să instalați Microsoft 365 Apps for enterprise pe RDS din centrul de administrare Microsoft 365, ***care utilizează setările implicite de instalare,*** utilizați următorii pași:

1.    Verificați ce abonament aveți. [Aflați cum](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Dacă este necesar, treceți la un alt abonament. [Aflați cum](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Dacă Office este deja instalat pe serverul RDS utilizând orice alte abonamente Microsoft, dezinstalați-l. De exemplu, accesăm **Panoul de control** > **Dezinstalarea unui program**. Dezinstalați utilizând [Asistentul de asistență și recuperare Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă aveți probleme.
4.    Pe serverul RDS, conectați-vă la centrul de administrare Microsoft 365 cu contul de administrator și [instalați Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    După instalarea Office, ***nu deschideți sau conectați-vă*** la nicio aplicații Office.
6.    Pe serverul RDS, activați activarea computerului partajat prin editarea registry urmând acești pași:
   1. Faceți clic cu butonul din dreapta pe butonul Windows din colțul din stânga jos al ecranului și selectați **Executare**. În caseta Deschidere, tastați **regedit**, apoi selectați **OK**.
   2. Selectați **Da** atunci când vi se solicită să permiteți Registry Editor să efectueze modificări pe dispozitiv.
   3. În Registry Editor, adăugați o valoare șir de **SharedComputerLicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Pe serverul RDS, ***conectați-vă ca utilizator final*** și [verificați dacă activarea computerului partajat este activată pentru Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

