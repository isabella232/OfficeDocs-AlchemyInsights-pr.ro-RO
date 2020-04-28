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
ms.openlocfilehash: 5a510f1137c7c49cd1de3d3fd2a470759e37ba1e
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908716"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limita de e-mail zilnică depășită. Fluxul de lucru este suspendat.

Această eroare poate fi primită în următoarele scenarii:

- Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă de flux de lucru SharePoint 2010 sau SharePoint 2013.
- Fluxul de lucru este configurat să trimită un mesaj de poștă electronică particularizat la mai mult de 200 de utilizatori la un moment dat, mai mult de 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.
- Când executați fluxul de lucru, mesajul de poștă electronică nu este trimis și observați următorul comportament:
    - Pentru un flux de lucru utilizând tipul de platformă SharePoint 2013, navigați la pagina **stare flux de lucru.** Pe pagina Stare flux de lucru, **starea internă** este setată la **Pornit**, iar balonul de informații se afișează Imposibil de trimis **unui destinatar**.

Pentru a rezolva această problemă, configurați fluxul de lucru pentru a trimite mesaje de poștă electronică fără a depăși [limitele expeditorului Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). De exemplu, utilizați o pauză în fluxul de lucru, trimiteți e-mailul la un grup Microsoft 365, la un grup de distribuire sau la un grup de securitate activat pentru e-mail sau trimiteți mesajul la mai puțin de 200 de destinatari la un moment dat.


Pentru mai multe informații, consultați următorul [articol](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Subiecte asociate
- [Creare flux](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și Flux](https://flow.microsoft.com/blog/sharepoint-and-flow/) 