---
title: Limita zilnică de e-mail a fost depășită. Fluxul de lucru este suspendat.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914663"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Limita de e-mail zilnică a fost depășită. Fluxul de lucru este suspendat.

Această eroare poate fi primită în următoarele scenarii:

- Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă de flux de lucru SharePoint 2010 sau SharePoint 2013.
- Fluxul de lucru este configurat să trimită un mesaj de e-mail particularizat către mai mult de 200 de utilizatori o dată, mai mult de 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.
- Atunci când rulați fluxul de lucru, mesajul de e-mail nu este trimis și observați următorul comportament:
    - Pentru un flux de lucru cu tipul SharePoint platformă 2013, navigați la pagina **Stare flux de** lucru. Pe pagina Stare flux de lucru, **Starea internă este** setată la **Început,** iar balonul de informații **afișează Nu se poate trimite unui destinatar.**

Pentru a ocoli această problemă, configurați fluxul de lucru pentru a trimite mesaje de e-mail fără a [depăși Exchange Online de expeditor.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) De exemplu, utilizați o pauză în fluxul de lucru, trimiteți mesajul de e-mail către un grup Microsoft 365, un grup de distribuire sau un grup de securitate cu e-mail activat sau trimiteți mesajul la mai puțin de 200 de destinatari odată.


Pentru mai multe informații, consultați următorul [articol.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Subiecte asociate
- [Crearea Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint și Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 