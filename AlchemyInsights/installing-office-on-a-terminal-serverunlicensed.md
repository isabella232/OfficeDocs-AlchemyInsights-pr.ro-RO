---
title: Instalarea biroului pe un Terminal Server - Fără licență
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763229"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalarea Office pe un Terminal Server

Pentru implementarea Microsoft 365 Apps for enterprise pe un Windows Server utilizând Remote Desktop Services (RDS), denumit anterior Terminal Services:
  
- Trebuie să aveți un abonament Microsoft 365 care include Microsoft 365 Apps for enterprise, ar fi Office 365 Enterprise E3 sau Enterprise E5. Planurile Microsoft 365 Apps for business și Microsoft 365 Apps for business Premium nu includ Microsoft 365 Apps for enterprise.

- Trebuie să activați [activarea computerului partajat](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Dacă doriți să instalați Microsoft 365 Apps for enterprise pe RDS din centrul de administrare Microsoft 365, ***care utilizează setările implicite de instalare,*** utilizați următorii pași.

> [!TIP]
> De asemenea, puteți descărca și executa [Asistentul de asistență și recuperare Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pentru a instala Microsoft 365 Apps for enterprise în modul de activare a computerului partajat.
  
1. Verificați ce abonament Microsoft 365 aveți. [Aflați](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Dacă este necesar, comutați la un alt abonament Microsoft 365. [Aflați](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Dacă Office este deja instalat pe serverul RDS utilizând orice alte abonamente Microsoft 365, dezinstalați-l. De exemplu, accesăm \> Control Panel Uninstall a program. Dezinstalați utilizând [Asistentul de asistență și recuperare Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă aveți probleme.

4. Pe serverul RDS, conectați-vă la centrul de administrare Microsoft 365 cu contul de administrator și [instalați Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. După instalarea Office, ***nu deschideți sau conectați-vă*** la nicio aplicații Office.

6. Pe serverul RDS, activați activarea computerului partajat prin editarea registry urmând acești pași:

1. Faceți clic cu butonul din dreapta pe butonul Windows din colțul din stânga jos al ecranului și selectați Executare. În caseta Deschidere, tastați **regedit**, apoi selectați OK.

2. Selectați Da atunci când vi se solicită să permiteți Registry Editor să efectueze modificări pe dispozitiv.

3. În Registry Editor, adăugați o valoare șir de **SharedComputerLicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Pe serverul RDS, ***conectați-vă ca utilizator final*** și [verificați dacă activarea computerului partajat este activată pentru Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Pentru mai multe detalii despre cerințele preliminare, instrucțiunile de instalare și instrucțiuni privind instalările particularizate utilizând Instrumentul de implementare Office, consultați [Implementarea aplicațiilor Microsoft 365 pentru întreprinderi utilizând Serviciile Desktop la distanță](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Pentru a remedia erorile legate de activarea computerului partajat, consultați [Depanarea problemelor cu activarea computerului partajat pentru Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  