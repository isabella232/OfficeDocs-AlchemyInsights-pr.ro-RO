---
title: Probleme de conexiune SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840563"
---
# <a name="sharepoint-designer-connection-issues"></a>Probleme de conexiune SharePoint Designer 

În cazul în care SharePoint Designer se confruntă cu probleme de conectare la site-uri SharePoint, încercați următoarele soluții comune.

Pasul 1: Verificaţi că SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) şi [2 august 2016 Update pentru SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Pasul 2: Şterge fişierele cache-ul local:

1. Închide SharePoint Designer 2013.

2. Pe computerul local, eliminaţi toate fişierele găsite în fiecare din următoarele foldere.

    - %AppData%\Microsoft\Web server Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Deschide SharePoint Designer 2013 şi introduceţi contul din nou pentru a vedea dacă funcţionează.

Pasul 3: [activa autentificarea moderne pentru Office 2013 pe Windows dispozitive](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Pasul 4: Administratorii va trebui să **Permite script-ul personalizat** în setările de centru de administrare SharePoint pentru a permite conexiunea de SharePoint Designer. Vedea [permite sau împiedică script-ul personalizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informaţii.


