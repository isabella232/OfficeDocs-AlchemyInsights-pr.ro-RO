---
title: Doar în citire pentru întreținere mesaj atunci când încercați să utilizați SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051293"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Doar în citire pentru întreținere mesaj atunci când încercați să utilizați SharePoint sau OneDrive

Utilizatorii pot primi un mesaj **doar în citire pentru întreținere** atunci când încercați să utilizați SharePoint sau OneDrive pentru unul dintre următoarele scenarii. 

-   O activitate de întreținere planificată sau activă.  Verificați-le navigând la [Centrul de mesaje](https://portal.office.com/adminportal/home#/messagecenter).
-   Un incident de serviciu activ, de înaltă prioritate, care poate apărea. Verificați pentru orice recomandări/incidente prin navigarea la [serviciul de sănătate](https://portal.office.com/adminportal/home#/servicehealth).
-   Un minor auto-vindecare scenariu de recuperare care ar putea fi întâmplă din cauza oricăror evenimente neașteptate pe serverele care ar putea dura mai puțin de 30 min sau cam asa ceva. 
    
    Nu există mesaje centrul de mesaje sau servicii de sănătate pentru aceste recuperări minore, dar ar trebui să fie înapoi la normal foarte curând.

În foarte puține ocazii am observat că unul dintre cele trei scenarii enumerate mai sus au fost cauza, și serviciul a fost restaurat, dar cache-ul utilizatorilor browser-ul nu a fost clarificat.

Vă rugăm să încercați să goliți memoria cache a browserului înainte de a naviga pe site.

1. În browserul Microsoft Edge, selectați **Setări**, apoi selectați **confidențialitate și securitate**.
2. Sub **Navigare clară**, selectați **Alegeți ce să goliți**.
3. Selectați **cookie-uri și date salvate pe site-ul web**și selectați **Golire**.

>[!Note] 
> Acești pași pot diferi atunci când se utilizează alte browsere, ar fi Mozilla Firefox sau Google Chrome.

>[!Note] 
> O altă opțiune ar fi să deschideți site-ul SharePoint sau OneDrive într-o fereastră InPrivate nouă.