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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511556"
---
# <a name="sharepoint-designer-connection-issues"></a>Probleme de conexiune SharePoint Designer 

Dacă SharePoint Designer întâmpină probleme de conexiune la site-urile SharePoint, încercați următoarele soluții comune.

Pasul 1: Verificați că SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) și actualizarea 2 August [2016 pentru SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Pasul 2: Goliți fișierele cache locale:

1. Închideți SharePoint Designer 2013.

2. Pe computerul local, eliminați toate fișierele găsite în fiecare dintre următoarele foldere.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\Web Server Extensions\Cache %APP
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Deschideți SharePoint Designer 2013 și introduceți din nou contul pentru a vedea dacă funcționează.

Pasul 3: [Activați autentificarea modernă pentru Office 2013 pe dispozitive Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Pasul 4: Administratorii vor trebui să **permită scriptul personalizat** în setările Centrului de administrare SharePoint pentru a permite conexiunea SharePoint Designer. Consultați [Permiterea sau împiedicarea scriptului particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informații.


