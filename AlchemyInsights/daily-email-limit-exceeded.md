---
title: Limita zilnică de e-mail depășită. Fluxul de lucru este suspendat.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053129"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limită de e-mail zilnică depășită. Fluxul de lucru este suspendat.

Această eroare poate fi primită în următoarele scenarii:

- Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă SharePoint 2010 sau SharePoint 2013 flux de lucru.
- Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail personalizat la mai mult de 200 utilizatori la un moment dat, mai mult de 10.000 destinatari pe zi, sau mai mult de 30 de mesaje pe minut.
- Când executați fluxul de lucru, mesajul de poștă electronică nu este trimis și observați următorul comportament:
    - Pentru un flux de lucru utilizând tipul de platformă SharePoint 2013, navigați la pagina **stare flux de lucru** . Pe pagina stare flux de lucru, **starea internă** este setată la **început**și balonul de informații afișează **Imposibil de trimis la un destinatar**.

Pentru a rezolva această problemă, configurați fluxul de lucru pentru a trimite mesaje de poștă electronică fără a depăși [limitele expeditorului Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). De exemplu, utilizați o pauză în fluxul de lucru, trimiteți e-mailul la un grup de 365 Office, un grup de distribuire sau un grup de securitate activat pentru e-mail sau trimiteți mesajul la mai puțin de 200 destinatari la un moment dat.


Pentru mai multe informații, consultați următorul [articol](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Subiecte asociate
- [Creare flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 