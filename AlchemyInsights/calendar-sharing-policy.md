---
title: 618 Politica de partajare a calendarului
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373011"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Eroare de politică la partajarea unui calendar

1. Efectuați una dintre următoarele acțiuni, în funcție de situația dvs.:
    - Conectați-vă la Exchange Online utilizând Remote PowerShell. Pentru mai multe informații, consultați [Conectarea la Exchange Online utilizând Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Pe serverul local, deschideți Componentă de administrare Exchange.
2. Determinați politica de partajare care este atribuită utilizatorului. Pentru aceasta, executați următoarea comandă și notați politica returnată:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Actualizați politica de partajare pentru utilizator. Pentru a proceda astfel, urmați acești pași:
    - Deschideți centrul de administrare Exchange.
    - Faceți clic pe **Organizație**, apoi faceți dublu clic pe politica atribuită utilizatorului sub **Partajare individuală**. Aceasta este politica care a fost returnată în pasul 2.
    - Pe pagina Regulă partajare, selectați nivelul de partajare a calendarului pe care doriți să îl permiteți sub **Specificați ce informații doriți să partajați;** faceți clic pe **Salvare**.

Pentru mai multe informații, [consultați: "Politica nu permite acordarea permisiunilor la acest nivel la unul sau mai multe dintre destinatarii" eroare atunci când utilizatorul încearcă să partajeze calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
