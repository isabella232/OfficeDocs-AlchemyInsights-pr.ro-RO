---
title: Doar în citire pentru mesajul de întreținere atunci când încercați să utilizați SharePoint sau OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670844"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Doar în citire pentru mesajul de întreținere atunci când încercați să utilizați SharePoint sau OneDrive

Utilizatorii pot primi un mesaj **doar în citire pentru întreținere** atunci când încearcă să utilizeze SharePoint sau OneDrive pentru unul dintre următoarele scenarii. 

-   O activitate de întreținere planificată sau activă.  Verificați dacă navigați la [Centrul de mesaje](https://portal.office.com/adminportal/home#/messagecenter).
-   Un incident de serviciu activ, prioritar, care poate apărea. Căutați recomandări/incidente navigând la [starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).
-   Un scenariu minor de recuperare automată care s-ar putea întâmpla din cauza oricăror evenimente neașteptate de pe serverele care pot dura mai puțin de 30 de minute. 
    
    Nu există niciun centru de mesaje sau posturi de stare a serviciului pentru aceste recuperări minore, dar ar trebui să reveniți la normal foarte curând.

În foarte puține ocazii am observat că una dintre cele trei scenarii listate mai sus a fost cauza, iar serviciul a fost restaurat, dar memoria cache a browserului utilizatori nu a fost eliminată.

Încercați să debifați memoria cache a browserului înainte de a naviga la site.

1. În browserul Microsoft Edge, selectați **Setări**, apoi selectați **confidențialitate și securitate**.
2. Sub **Ștergere navigare**, selectați **Alegeți ce să goliți**.
3. Selectați **modulele cookie și datele salvate ale site-urilor web**și selectați **Ștergere**.

>[!Note] 
> Acești pași pot diferi atunci când utilizați alte browsere, cum ar fi Mozilla Firefox sau Google Chrome.

>[!Note] 
> O altă opțiune ar fi să deschideți site-ul SharePoint sau OneDrive într-o fereastră inprivată nouă.