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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529031"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Evenimentul OnChange nu se produce dacă câmpul este modificat prin programare

Evenimentul *onChange* nu se produce dacă câmpul se modifică prin programare utilizând *atributul.* metoda [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Dacă doriți ca rutine de eveniment pentru Evenimentul *onChange* pentru a executa după ce setați valoarea trebuie să utilizați *atributul formcontext. data. entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metoda în codul dvs.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
