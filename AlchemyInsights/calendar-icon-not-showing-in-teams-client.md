---
title: Pictograma Calendar nu e afișată în clientul Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989603"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Pictograma Calendar nu e afișată în clientul Teams

Fila Calendar din Teams necesită acces la o cutie poștală Exchange via Exchange Web Services. Cutia poștală Exchange poate fi Online sau La-Locație. Pentru utilizatorii Online care nu văd Fila Calendar, asigurați-vă că acestea [sunt licențiate pentru o cutie poștală Exchange Online, iar cutia poștală este activată](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Dacă un utilizator are o cutie poștală validă în Exchange Online, dar tot nu poate vedea Fila Calendar, este posibil să întâmpinați o problemă de rețea. Utilizați [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) și rulați **Testele de Conectivitate Microsoft Exchange Web Services** pentru utilizatorul afectat.

În cele din urmă, verificați aplicațiile [Teams Apps - politicile de instalare a aplicațiilor](https://admin.teams.microsoft.com/policies/app-setup) pentru a vă asigura că aplicația Calendar nu a fost eliminată din politica aplicată utilizatorului (cel mai probabil, **Global (implicit la nivel de Organizație)**.

Dacă utilizatorii dvs. au domiciliul La-Locație, trebuie să confirmați că este sănătoasă configurația hibridă. Utilizați [Expertul de Configurare Hibridă ](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pentru a depana.

Rețineți că [Teams necesită Exchange 2016 CU3 sau o versiune mai recentă](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
