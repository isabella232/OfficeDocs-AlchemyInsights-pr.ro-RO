---
title: Instalarea office pe un Server Terminal - fără licenţă
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307312"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalarea Office pe un Server Terminal

Pentru implementarea Office 365 ProPlus pe un Windows Server folosind Remote Desktop servicii (RDS), fostă numit Terminal Services:
  
- Trebuie să aveţi un plan de Office 365 care include Office 365 ProPlus, cum ar fi Office 365 Intreprindere E3 sau Intreprindere E5. Planuri Office 365 Business si Office 365 Business Premium nu includ Office 365 ProPlus.
    
- Aveţi nevoie pentru a permite [Activarea shared calculator](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Dacă doriţi să instalaţi Office 365 ProPlus pe RDS la portalul Office 365 ** *care utilizează setările implicite ale instalării* **, urmaţi aceşti paşi: 
  
1. Verifica ce plan de Office 365 care aveţi. [Aflaţi cum](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Dacă este necesar, trecerea la o diferite Office 365 planul. [Aflaţi cum](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. În cazul în care biroul este deja instalat pe serverul RDS folosind orice alte planuri Office 365, dezinstalaţi-l. De exemplu, de a merge la panoul de Control \> dezinstala un program. Uninstall folosire [Microsoft Support si asistent de recuperare](https://aka.ms/SARA-OfficeUninstall-Alchemy) în cazul în care se execută în probleme. 
    
4. Pe serverul RDS, faceţi sign in la portalul Office 365 cu contul de administrator şi [instala Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. După ce este instalat Office, ** *nu deschide sau conectaţi-vă* ** pentru orice aplicatii de birou. 
    
6. Pe serverul RDS, permite activarea computer partajat prin editarea registry urmând aceşti paşi:
    
1. Faceţi clic dreapta pe butonul de Windows în colţul din stânga jos a ecranului, şi selectaţi Executare. În Deschidere cutie, tip **regedit**, şi apoi selectaţi OK. 
    
2. Selectați Da când vi se solicită să permită Registry Editor pentru a face modificări la aparatul dvs.
    
3. În Registry Editor, adăugaţi o valoare şir de **SharedComputerLicensing** cu o setare de 1 sub HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Pe serverul RDS, ** *conectaţi-vă ca un utilizator final* ** şi [să verifice că shared calculator activation is enabled pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Pentru mai multe detalii pe premise, instrucţiuni de configurare şi îndrumări cu privire la instalări particularizate utilizând instrumentul de implementare Office, vă rugăm să consultaţi [Implementaţi Office 365 ProPlus folosind Remote Desktop servicii](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Pentru a rezolva erorile legate de shared calculator activare, vă rugăm să consultaţi [Depanarea problemelor cu activare shared calculator pentru Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

