---
title: Site-ul modernă ca site-ul rădăcină
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057759"
---
# <a name="modern-site-as-root-site"></a>Site-ul modernă ca site-ul rădăcină

[Lansare ţintă](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) clienţii pot permite acum experienţă de site-ul moderne de comunicare la site-ul clasic rădăcină lor chiriaş de SharePoint.

Această caracteristică poate fi activată prin rularea un cmdlet PowerShell simplu. La executarea cu succes a PowerShell command(s), site-ul rădăcină va avea o nouă comunicare-site-ul initiala. Detalii despre cerinţele PowerShell cmdlet şi caracteristică sunt disponibile în articol [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Ne va fi treptat rulare acest lucru, off implicit, orientate versiune clienţilor în 2019 mai devreme, şi rola vor fi disponibile în întreaga lume, până la sfârşitul lunii iunie 2019. Continua să se refere la [Centru de mesaje](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) pentru alte caracteristici noi cu cel Modern. 

**Important**: nu ştergeţi site-ul clasic rădăcină pentru a crea un Site de comunicare moderne. Acest lucru nu este acceptată de Microsoft. Ştergerea site-ul rădăcină va face toate site-urile SharePoint din organizaţie inaccesibile pentru toţi utilizatorii, până la restaurarea site-ul sau de a crea un site nou la aceeaşi adresă URL. 
 
 