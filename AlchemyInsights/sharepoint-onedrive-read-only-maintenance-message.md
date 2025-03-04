---
title: Read-Only pentru mesajul de întreținere atunci când încercați să utilizați SharePoint sau OneDrive
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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329460"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only pentru mesajul de întreținere atunci când încercați să utilizați SharePoint sau OneDrive

Utilizatorii pot primi **un mesaj Doar** în citire pentru întreținere atunci când încearcă să utilizeze SharePoint sau OneDrive pentru unul dintre scenariile următoare. 

-   O activitate de întreținere planificată sau activă.  Verificați-le navigând la Centrul [de mesaje](https://portal.office.com/adminportal/home#/messagecenter).
-   Un incident de serviciu activ, de înaltă prioritate, care poate apărea. Căutați orice consultanță/incident, navigând la Starea [serviciilor.](https://portal.office.com/adminportal/home#/servicehealth)
-   Un scenariu minor de recuperare automată ce poate avea loc din cauza oricăror evenimente neașteptate pe servere, care poate dura mai puțin de 30 de minute sau mai mult. 
    
    Nu există nicio postare în Centrul de mesaje sau Starea serviciilor pentru aceste recuperare minore, dar ar trebui să reveniți la normal foarte curând.

Cu foarte puține ocazii, am observat că unul dintre cele trei scenarii listate mai sus a fost cauza, iar serviciul a fost restaurat, dar memoria cache a browserului utilizatorilor nu a fost golită.

Încercați să goliți memoria cache a browserului înainte de a naviga la site.

1. În browserul Microsoft Edge, selectați **setări Setări**, apoi selectați **Confidențialitate și securitate**.
2. Sub **Golire navigare**, selectați **Alegeți ce să goliți**.
3. Selectați **Module cookie și date salvate din site-ul** web și **selectați Golire**.

**Notă:** Acești pași pot diferi atunci când utilizați alte browsere, cum ar fi Mozilla Firefox sau Google Chrome.

**Notă:** o altă opțiune ar fi să deschideți site-SharePoint de e-OneDrive într-o fereastră InPrivate nouă.