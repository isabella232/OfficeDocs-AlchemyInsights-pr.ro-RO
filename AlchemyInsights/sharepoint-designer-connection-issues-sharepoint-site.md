---
title: SharePoint Probleme de conexiune cu Proiectant
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942037"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Probleme de conexiune cu Proiectant 

Dacă SharePoint Designer se confruntă cu probleme de conexiune la SharePoint-uri, încercați următoarele soluții comune.

Pasul 1: Verificați dacă SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) și Actualizarea din 2 august [2016 pentru SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Pasul 2: Goliți fișierele cache locale:

1. Închideți SharePoint Designer 2013.

2. Pe computerul local, eliminați toate fișierele din fiecare dintre următoarele foldere.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Deschideți SharePoint Designer 2013 și introduceți din nou contul pentru a vedea dacă funcționează.

Pasul 3: [Activați autentificarea modernă pentru Office 2013 pe Windows dispozitive .](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Pasul 4: Administratorii vor trebui să permită **script** particularizat în setările SharePoint de administrare pentru a permite SharePoint Designer. Consultați [Permiterea sau prevenirea scriptului particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informații.


