---
title: Dynamics 365 formulare reguli de afaceri-regulă de afaceri nu de ardere pentru un formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769351"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Evenimentul OnChange nu se produce dacă câmpul este modificat prin programare

Evenimentul *onChange* nu se produce dacă câmpul se modifică prin programare utilizând *atributul.* metoda [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Dacă doriți ca rutine de eveniment pentru Evenimentul *onChange* pentru a executa după ce setați valoarea trebuie să utilizați metoda *formcontext. data. Entity atributul* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) în codul.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
