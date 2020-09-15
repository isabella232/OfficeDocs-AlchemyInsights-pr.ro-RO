---
title: Politica de partajare a calendarelor 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684242"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Eroare de politică la partajarea unui calendar

1. Faceți una dintre următoarele acțiuni, în funcție de situația dvs.:
    - Conectați-vă la Exchange Online folosind PowerShell la distanță. Pentru mai multe informații, consultați [conectarea la Exchange Online folosind PowerShell la distanță](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Pe serverul local, deschideți componenta de administrare Exchange.
2. Determinați Politica de partajare atribuită utilizatorului. Pentru a face acest lucru, derulează următoarea comandă și notați politica returnată:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Actualizați Politica de partajare pentru utilizator. Pentru a proceda astfel, urmați acești pași:
    - Deschideți Centrul de administrare Exchange.
    - Faceți clic pe **organizație**, apoi faceți dublu clic pe politica atribuită utilizatorului sub **Partajare individuală**. Aceasta este politica care a fost returnată în pasul 2.
    - Pe pagina regulă de partajare, selectați nivelul de partajare a calendarului pe care doriți să-l permiteți sub **specificarea informațiilor pe care doriți să le partajați**; Faceți clic pe **Salvare**.

Pentru mai multe informații, consultați: ["Politica nu permite acordarea permisiunilor la acest nivel la una sau mai multe dintre aceste erori" atunci când utilizatorul încearcă să partajeze calendarul](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
