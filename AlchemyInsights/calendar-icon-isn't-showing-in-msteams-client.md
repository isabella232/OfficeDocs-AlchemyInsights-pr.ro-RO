---
title: Pictograma Calendar nu se afișează în Microsoft Teams client
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120016"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Pictograma Calendar nu se afișează în Microsoft Teams client

Fila **Calendar** din Teams necesită acces la o cutie poștală Exchange prin Exchange Web Services. Cutia Exchange poștală poate fi online sau locală. Pentru utilizatorii online care nu văd fila **Calendar,** asigurați-vă că aceștia sunt licențiați pentru [o cutie poștală de Exchange Online și cutia poștală este activată.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Dacă utilizatorii dvs. sunt acasă, local, trebuie să confirmați că configurația hibridă este în bună stare. Utilizați [Expertul de Configurare Hibridă ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pentru a depana. Rețineți că [Teams necesită Exchange 2016 CU3 sau o versiune mai recentă](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Pentru mai multe informații și pași de depanare, consultați [Depanarea problemelor Microsoft Teams și Exchange Server de interacțiune cu utilizatorul.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
