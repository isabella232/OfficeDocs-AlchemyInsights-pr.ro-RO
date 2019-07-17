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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748483"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Eveniment OnChange nu se produce în cazul în care câmpul este schimbat programatic

Eveniment *OnChange* nu se produce în cazul în care câmpul este schimbată folosind programatic *atribut.* metoda [SetareValoare](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Dacă doriţi gestionari de eveniment pentru eveniment *OnChange* pentru a rula după ce setaţi valoarea pe care trebuie să utilizaţi *atribut formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metoda în codul dumneavoastră.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
