---
title: Instalarea Office pe un terminal server-fără licență
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205421"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalarea Office pe un server terminal

Pentru implementarea Office 365 ProPlus pe un Windows Server utilizând consolidare servicii Desktop la distanță (RDS), denumit anterior Terminal Services:
  
- Trebuie să aveți un plan Office 365 care include Office 365 ProPlus, ar fi Office 365 Enterprise E3 sau Enterprise E5. Planurile Office 365 Business și Office 365 Business Premium nu includ Office 365 ProPlus.

- Trebuie să activați [activarea computerului partajat](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Dacă doriți să instalați Office 365 ProPlus pe RDS de la centrul de administrare Microsoft 365, ***care utilizează setările de instalare implicite***, utilizați pașii următori.

> [!TIP]
> De asemenea, aveți posibilitatea să descărcați și să executați [Asistentul Microsoft pentru asistență și recuperare](https://aka.ms/SaRA_OfficeSCA_M365Portal) pentru a instala Office 365 ProPlus în modul de activare a computerului partajat.
  
1. Verificați ce Office 365 plan aveți. [Aflați](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Dacă este necesar, comutați la un alt plan Office 365. [Aflați](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Dacă Office este deja instalat pe serverul RDS utilizând orice alte planuri de Office 365, dezinstalați-l. De exemplu, mergând la panoul \> de control Dezinstalați un program. Dezinstalați utilizând [asistența Microsoft și asistentul de recuperare](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă executați probleme.

4. Pe serverul RDS, conectați-vă la centrul de administrare Microsoft 365 cu contul de administrator și [Instalați Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. După ce Office este instalat, ***nu deschideți sau faceți sign in*** la orice aplicații Office.

6. Pe serverul RDS, activați activarea computerului partajat editând registry urmând acești pași:

1. Faceți clic dreapta pe butonul Windows din colțul din stânga jos al ecranului și selectați executare. În caseta Deschidere, tastați **regedit**, apoi selectați OK.

2. Selectați Da când vi se solicită să permiteți Registry Editor să facă modificări pe dispozitiv.

3. În editorul de registry, adăugați o valoare șir de **Sharedcomputerlicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Pe serverul RDS, ***Conectați-vă ca utilizator final*** și [Verificați că activarea computerului partajat este activată pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Pentru mai multe detalii despre cerințe preliminare, instrucțiuni de instalare și îndrumare pe instalări particularizate utilizând instrumentul de implementare Office, consultați [implementarea office 365 ProPlus utilizând consolidare servicii Desktop la distanță](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Pentru a remedia erorile legate de activarea computerului partajat, consultați [Depanarea problemelor cu activarea computerului partajat pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  