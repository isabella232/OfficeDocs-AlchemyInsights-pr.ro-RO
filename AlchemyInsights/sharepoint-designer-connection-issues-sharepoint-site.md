---
title: Nivelurile de permisiune SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760704"
---
# <a name="sharepoint-designer-connection-issues"></a>Probleme de conexiune SharePoint Designer 

Dacă SharePoint Designer se confruntă cu probleme de conectare la site-uri SharePoint, vă rugăm să încercaţi următoarele soluţii comune.

Pasul 1: Verificaţi dacă SharePoint Designer este actualizat.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Update pentru SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Pasul 2: Şterge fişierele cache-ul local

- Închide SharePoint Designer 2013.

- Pe computerul local, navigaţi la următoarele foldere pentru a elimina fişiere în cache.

- Faceţi clic pe Start, Run şi şterge toate fişierele găsite în fiecare dintre locaţiile de mai jos.

%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Deschide SharePoint Designer 2013 şi introduceţi contul din nou pentru a vedea dacă funcţionează.

Pasul 3: [activa autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Pasul 4: Administratorii va trebui să permite script-ul personalizat pentru a permite conexiunea de SharePoint Designer.

Pentru măsurile detaliate, exemple şi consideraţii [permite sau împiedică script-ul personalizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


