---
title: Limita zilnică de e-mail depășită. Fluxul de lucru este suspendat.
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
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731575"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limita zilnică de e-mail depășită. Fluxul de lucru este suspendat.

Această eroare poate fi primită în următoarele scenarii:

- Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă de flux de lucru SharePoint 2010 sau SharePoint 2013.
- Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail particularizat la mai mult de 200 de utilizatori la un moment dat, mai mult de 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.
- Atunci când rulează fluxul de lucru, mesajul de e-mail nu este trimis și observați următorul comportament:
    - Pentru un flux de lucru utilizând tipul de platformă SharePoint 2013, navigați la pagina **stare flux de lucru** . În pagina stare flux de lucru, **starea internă** este setată la **început**și balonul de informații **nu se afișează în imposibilitatea de a-l trimite unui destinatar**.

Pentru a rezolva această problemă, configurați fluxul de lucru pentru a trimite mesaje de e-mail fără a depăși [limitele expeditorului Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). De exemplu, utilizați o pauză în fluxul de lucru, trimiteți e-mailul la un grup Microsoft 365, la un grup de distribuire sau la un grup de securitate cu e-mail activat sau trimiteți mesajul la mai puțin de 200 de destinatari odată.


Pentru mai multe informații, consultați [articolul](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)următor.

## <a name="related-topics"></a>Subiecte asociate
- [Crearea fluxului](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și fluxul](https://flow.microsoft.com/blog/sharepoint-and-flow/) 