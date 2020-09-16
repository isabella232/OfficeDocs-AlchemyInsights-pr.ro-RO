---
title: Probleme de conexiune SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727183"
---
# <a name="sharepoint-designer-connection-issues"></a>Probleme de conexiune SharePoint Designer 

Dacă SharePoint Designer întâmpină probleme de conexiune la site-urile SharePoint, încercați următoarele soluții comune.

Pasul 1: Verificați dacă SharePoint Designer 2013 este actualizat cu [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) și [actualizarea din 2 august 2016 pentru SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Pasul 2: debifați fișierele din memoria cache locală:

1. Închideți SharePoint Designer 2013.

2. Pe computerul local, eliminați toate fișierele găsite în fiecare dintre următoarele foldere.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Deschideți SharePoint Designer 2013 și introduceți contul din nou pentru a vedea dacă funcționează.

Pasul 3: [activați autentificarea modernă pentru Office 2013 pe dispozitivele Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Pasul 4: administratorii vor trebui să **permită un script particularizat** în setările din centrul de administrare SharePoint, pentru a permite conexiunea SharePoint Designer. Consultați [permiterea sau prevenirea scriptului particularizat](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pentru mai multe informații.


