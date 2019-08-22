---
title: Dynamics 365 formează regulilor de afaceri - afaceri regula nu de tragere pentru o formă
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529031"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Eveniment OnChange nu se produce în cazul în care câmpul este schimbat programatic

Eveniment *OnChange* nu se produce în cazul în care câmpul este schimbată folosind programatic *atribut.* metoda [SetareValoare](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Dacă doriţi gestionari de eveniment pentru eveniment *OnChange* pentru a rula după ce setaţi valoarea pe care trebuie să utilizaţi *atribut formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metoda în codul dumneavoastră.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
