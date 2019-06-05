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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716903"
---
# <a name="sharepoint-designer-connection-issues"></a>Probleme de conexiune SharePoint Designer 

<p>Dacă SharePoint Designer se confruntă cu probleme de conectare la site-uri SharePoint, vă rugăm să încercaţi următoarele soluţii comune.</p> <p><strong>Pasul 1:</strong> <strong>Verifica SharePoint Designer este actualizat&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Update pentru SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Pasul 2:</strong> <strong>Şterge fişierele cache-ul local</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Închide SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Pe computerul local, navigaţi la următoarele foldere pentru a elimina fişiere în cache.&nbsp;</li> <li style="font-weight: 400;">Faceţi clic pe <strong>Start -&gt; a alerga</strong> şi şterge toate fişierele găsite în fiecare dintre locaţiile de mai jos.&nbsp;<br /><br />%AppData%\Microsoft\Web server Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Deschide SharePoint Designer 2013 şi introduceţi contul din nou pentru a vedea dacă funcţionează.</li> </ol> <p><strong>Pasul 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Activa autentificarea moderne pentru Office 2013 pe Windows dispozitive</strong></a>&nbsp;</p> <p><strong>Pasul 4:</strong> <strong>Administratorii va trebui să permite Custom script-ul pentru a permite conexiunea de SharePoint Designer</strong>.</p> <p>Pentru măsurile detaliate, exemple şi consideraţii <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">permite sau împiedică script-ul personalizat</a>.&nbsp;</p>


