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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="bb319-102">Eveniment OnChange nu se produce în cazul în care câmpul este schimbat programatic</span><span class="sxs-lookup"><span data-stu-id="bb319-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="bb319-103">Eveniment *OnChange* nu se produce în cazul în care câmpul este schimbată folosind programatic *atribut.* metoda [SetareValoare](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="bb319-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="bb319-104">Dacă doriţi gestionari de eveniment pentru eveniment *OnChange* pentru a rula după ce setaţi valoarea pe care trebuie să utilizaţi *atribut formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metoda în codul dumneavoastră.</span><span class="sxs-lookup"><span data-stu-id="bb319-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
