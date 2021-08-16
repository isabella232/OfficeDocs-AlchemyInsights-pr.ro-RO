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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031490"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Implementarea Aplicații Microsoft 365 pentru întreprindere pentru utilizare partajată pe RDS, Terminal Server sau VDI

Pentru a Aplicații Microsoft 365 pentru întreprindere servicii desktop la distanță (RDS), denumite anterior Terminal Services:

- Trebuie să aveți un plan Microsoft 365 For Business sau un plan Office 365 care include Aplicații Microsoft 365 pentru întreprindere, cum ar fi Office 365 Enterprise E3 sau Enterprise E5.
   > [!NOTE]
   > Planurile Aplicații Microsoft 365 pentru afaceri și Microsoft 365 Business Standard de date nu includ Aplicații Microsoft 365 pentru întreprindere.
- Trebuie să activați [activarea computerului partajat.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> De asemenea, puteți să descărcați și să [rulați Microsoft Asistent pentru recuperare și asistență](https://aka.ms/SaRA_OfficeSCA_M365Portal) a instala Aplicații Microsoft 365 pentru întreprindere în modul de activare a computerului partajat.

Pentru mai multe informații despre cerințele preliminare, instrucțiunile de configurare și instrucțiunile pentru instalările particularizate utilizând Instrumentul de implementare Office, consultați [Implementarea Aplicații Microsoft 365 pentru întreprindere](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)utilizând servicii desktop la distanță.

Pentru a remedia erorile legate de activarea computerului partajat:

- Consultați [Depanarea problemelor cu activarea computerului partajat pentru Aplicații Microsoft 365 pentru întreprindere](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Consultați [Resetarea aplicațiilor Microsoft 365 pentru starea de activare pentru întreprinderi](https://go.microsoft.com/fwlink/?linkid=2109218).

Dacă doriți să instalați pe RDS Aplicații Microsoft 365 pentru întreprindere pe Centru de administrare Microsoft 365, care utilizează setările de ***instalare implicite,*** urmați acești pași:

1. Verificați ce abonament aveți. [Aflați cum](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Dacă este necesar, comutați la alt abonament. [Aflați cum](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Dacă Office este instalat deja pe serverul RDS utilizând orice alte abonamente Microsoft, dezinstalați-l. De exemplu, accesând Panoul de **control**  >  **Dezinstalați un program.** Dezinstalați [utilizând Microsoft Asistent pentru recuperare și asistență](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă aveți probleme.
4. Pe serverul RDS, conectați-vă la Centru de administrare Microsoft 365 cu contul de administrator și [instalați Aplicații Microsoft 365 pentru întreprindere](https://portal.office.com/OLS/MySoftware.aspx).
5. După Office instalare, ***nu deschideți aplicațiile și nu vă conectați*** la Office dvs.
6. Pe serverul RDS, activați activarea computerului partajat prin editarea registry, urmând acești pași:
   1. Faceți clic dreapta pe Windows din colțul din stânga jos al ecranului și selectați **Rulare**. În caseta Deschidere, tastați **regedit**, apoi selectați **OK**.
   2. Selectați **Da** atunci când vi se solicită să permiteți editorului de registry să facă modificări la dispozitivul dvs.
   3. În Registry Editor, adăugați o valoare șir de **date SharedComputerLicensing** cu setarea 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Pe serverul RDS, ***conectați-vă*** ca utilizator final și verificați dacă activarea computerului partajat este [activată pentru Aplicații Microsoft 365 pentru întreprindere](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
