---
title: Pictograma Calendar nu se afișează în clientul Microsoft teams
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
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583924"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Pictograma Calendar nu se afișează în clientul Microsoft teams

Fila **Calendar** din teams necesită acces la o cutie poștală Exchange prin Exchange Web Services. Cutia poștală Exchange poate fi online sau locală. Pentru utilizatorii online care nu văd fila **Calendar** , asigurați-vă că [sunt autorizați pentru o cutie poștală Exchange Online și că este activată cutia poștală](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Dacă utilizatorii sunt conectați local, trebuie să confirmați că configurația hibridă este sănătoasă. Utilizați [Expertul de Configurare Hibridă ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pentru a depana. Rețineți că [Teams necesită Exchange 2016 CU3 sau o versiune mai recentă](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Pentru mai multe informații și pași de depanare, consultați [Depanarea problemelor de interacțiune Microsoft teams și Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
