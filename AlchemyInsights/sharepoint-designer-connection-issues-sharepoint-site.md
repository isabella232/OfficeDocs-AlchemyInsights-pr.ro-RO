---
title: Probleme de conexiune SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051725"
---
# <a name="sharepoint-designer-connection-issues"></a>Probleme de conexiune SharePoint Designer 

Dacă SharePoint Designer se confruntă cu probleme de conexiune la site-uri SharePoint, vă rugăm să încercați următoarele soluții comune.

Pasul 1: Verificați că SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) și [2 august, 2016 actualizare pentru SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Pasul 2: goliți fișierele cache locale:

1. Închideți SharePoint Designer 2013.

2. Pe computerul local, eliminați toate fișierele găsite în fiecare dintre următoarele foldere.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Deschideți SharePoint Designer 2013 și introduceți din nou contul pentru a vedea dacă funcționează.

Pasul 3: [activați autentificarea modernă pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Pasul 4: administratorii vor trebui să **permită script particularizat** în setările centrului de administrare SharePoint pentru a permite conexiunea SharePoint Designer. Consultați [Permiteți sau împiedicați scriptul particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informații.


