---
title: Dynamics 365 Forms Business Rules - regulă de business care nu aplică pentru un formular
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947311"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Evenimentul OnChange nu are loc dacă câmpul este modificat prin program

Evenimentul *OnChange* nu are loc dacă câmpul este modificat prin program utilizând *atributul.* [metoda setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Dacă doriți ca gestionarele de evenimente pentru evenimentul *OnChange* să ruleze după ce setați valoarea, trebuie să utilizați metoda *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) în codul dvs.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
