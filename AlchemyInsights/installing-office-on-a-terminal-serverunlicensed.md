---
title: Instalarea office pe un Terminal Server - nelicențiată
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322011"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalarea Office pe un Terminal Server

Pentru implementarea Aplicații Microsoft 365 pentru întreprindere pe un Windows Server care utilizează Servicii desktop la distanță (RDS), denumit anterior Terminal Services:
  
- Trebuie să aveți un abonament Microsoft 365 care include Aplicații Microsoft 365 pentru întreprindere, cum ar fi Office 365 Enterprise E3 sau Enterprise E5. Planurile Aplicații Microsoft 365 pentru afaceri și Aplicații Microsoft 365 pentru afaceri Premium de date nu includ Aplicații Microsoft 365 pentru întreprindere.

- Trebuie să activați [activarea computerului partajat.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Dacă doriți să instalați RDS Aplicații Microsoft 365 pentru întreprindere pe RDS de pe Centru de administrare Microsoft 365, care utilizează setările de instalare ***implicite,*** urmați acești pași.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Verificați ce Microsoft 365 abonament aveți. [Aflați cum](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Dacă este necesar, comutați la alt Microsoft 365 abonament. [Aflați cum](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Dacă Office este instalat deja pe serverul RDS utilizând orice alte Microsoft 365 abonamente, dezinstalați-l. De exemplu, accesând Panoul de control \> Dezinstalați un program. Dezinstalați [utilizând Microsoft Asistent pentru recuperare și asistență](https://aka.ms/SARA-OfficeUninstall-Alchemy) dacă aveți probleme.

4. Pe serverul RDS, conectați-vă la Centru de administrare Microsoft 365 cu contul de administrator [și instalați Aplicații Microsoft 365 pentru întreprindere](https://portal.office.com/OLS/MySoftware.aspx).

5. După Office se instalează, ***nu deschideți aplicațiile*** și nu vă conectați la Office mele.

6. Pe serverul RDS, activați activarea computerului partajat prin editarea registry, urmând acești pași:

1. Faceți clic dreapta pe Windows din colțul din stânga jos al ecranului și selectați Rulare. În caseta Deschidere, tastați **regedit**, apoi selectați OK.

2. Selectați Da atunci când vi se solicită să permiteți editorului de registry să facă modificări la dispozitivul dvs.

3. În Registry Editor, adăugați o valoare șir de date **SharedComputerLicensing** cu o setare 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Pe serverul RDS, ***conectați-vă*** ca utilizator final și verificați dacă activarea computerului partajat este [activată pentru Aplicații Microsoft 365 pentru întreprindere](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Pentru mai multe detalii despre cerințele preliminare, instrucțiuni de configurare și instrucțiuni pentru instalările particularizate utilizând Instrumentul de implementare Office, consultați Implementarea Aplicații Microsoft 365 pentru întreprindere utilizând servicii desktop la [distanță.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Pentru a remedia erorile legate de activarea computerului partajat, consultați Depanarea problemelor [de activare a computerului partajat pentru Aplicații Microsoft 365 pentru întreprindere](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  