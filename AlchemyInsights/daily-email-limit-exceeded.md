---
title: Zi cu zi e-mail depăşit limita. Flux de lucru este suspendat.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059650"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>E-mail zilnic a depăşit limita. Flux de lucru este suspendat.

Această eroare poate fi primit în următoarele situaţii:

- Ai un flux de lucru SharePoint Online care utilizează SharePoint 2010 sau tipul de platforma de flux de lucru SharePoint 2013.
- Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail personalizate pentru mai mult de 200 de utilizatori la un moment dat, peste 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.
- Când executaţi fluxul de lucru, nu este trimis mesajul e-mail, şi observaţi următorul comportament:
    - Pentru un flux de lucru utilizând tipul de platforma SharePoint 2013, navigați la pagina **Stare flux de lucru** . Pe pagina stare flux de lucru, **Starea internă** este setată la **începute**şi balonul cu informaţii afişează **nu se poate trimite la un destinatar**.

Pentru a rezolva această problemă, configuraţi fluxul de lucru pentru a trimite mesaje e-mail, fără a depăşi [limitele de expeditor Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). De exemplu, utilizaţi o pauză în fluxul de lucru, trimiteţi un email la un grup de Office 365, un grup de distribuire sau un grup de securitate mail activat sau trimite mesajul la mai puţin de 200 de destinatari la un moment dat.


Pentru informaţii suplimentare, consultaţi următorul [articol](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Subiecte asociate
- [Crea fluxul](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint şi fluxul](https://flow.microsoft.com/blog/sharepoint-and-flow/) 