---
title: Controlul actualizărilor automate pentru aplicațiile Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439922"
---
# <a name="control-automatic-updates-for-office-apps"></a>Controlul actualizărilor automate pentru aplicațiile Office

În mod implicit, actualizările pentru Aplicații Office sunt descărcate automat și aplicate în fundal, fără nicio intervenție a utilizatorului. Cu toate acestea, administratorii pot controla modul în care se aplică actualizările utilizând setările Office Update. Setările de actualizare permit administratorilor să activeze sau să dezactiveze actualizările automate, să afișeze sau să ascundă butonul **Actualizare acum** în Office, să seteze termene de actualizare și multe altele. Pentru informații detaliate, consultați:

- [Configurarea setărilor de actualizare pentru Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Actualizarea automată pentru Office nu este activată](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definirea modului de actualizare a Office după instalare](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Pentru a revizui setările de actualizări existente aplicate unui computer client, urmați acești pași:

1. Deschideți Registry Editor accesând **Start**  >  **Run**  >  **regedit**.
2. Comutați la următoarea locație și revizuiți setările Office Update:  
    R. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    B. Faceți clic peToRun\Configurare

**Notă**  Dacă este setată cheia OfficeMgmtCOM, este posibil să vedeți mesajul "Actualizările sunt gestionate de administratorul de sistem" în Actualizări **Office**  >  **Account**  >  **Office**. Pentru mai multe informații, consultați [Gestionarea actualizărilor pentru aplicațiile Microsoft 365 cu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  