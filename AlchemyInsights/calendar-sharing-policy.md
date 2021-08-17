---
title: 618 Politica de partajare a calendarelor
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091615"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Eroare de politică la partajarea unui calendar

1. Faceți una dintre următoarele acțiuni, după cum este necesar pentru situația dvs.:
    - Conectare faceți Exchange Online, utilizând PowerShell la distanță. Pentru mai multe informații, [consultați Conectare utilizați Exchange Online PowerShell la distanță.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Pe serverul local, deschideți partea de administrare Exchange administrare.
2. Determinați politica de partajare atribuită utilizatorului. Pentru a face acest lucru, rulați următoarea comandă și notați politica returnată:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Actualizați politica de partajare pentru utilizator. Pentru a proceda astfel, urmați acești pași:
    - Deschideți centrul Exchange de administrare.
    - Faceți **clic** pe Organizație, apoi faceți dublu clic pe politica atribuită utilizatorului, sub Partajare **individuală.** Aceasta este politica returnată la pasul 2.
    - Pe pagina Regulă de partajare, selectați nivelul de partajare a calendarului pe care doriți să îl permiteți sub **Specificați ce informații doriți să partajați;** faceți **clic pe Salvare.**

Pentru mai multe informații, consultați: "Politica nu permite acordarea de permisiuni la acest nivel unuia sau mai mulți destinatari" atunci când utilizatorul încearcă să [partajeze calendarul.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
