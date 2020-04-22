---
title: 902 (Sincronizare erori din cauza obiectelor dublate)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767147"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="0cb0c-102">Sincronizareerori datorate obiectelor dublate</span><span class="sxs-lookup"><span data-stu-id="0cb0c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="0cb0c-103">Este posibil să primiți unul dintre următoarele mesaje de eroare atunci când sincronizaredirector se termină în Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="0cb0c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="0cb0c-104">Imposibil de actualizat acest obiect în Microsoft Online Services, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din directorul local.</span><span class="sxs-lookup"><span data-stu-id="0cb0c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="0cb0c-105">Un obiect sincronizat cu aceeași adresă proxy există deja în directorul Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="0cb0c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="0cb0c-106">Imposibil de actualizat acest obiect, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect în serviciile de director local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0cb0c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="0cb0c-107">Pentru a identifica și remedia problema, descărcați și executați [Instrumentul de remediere a erorilor IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="0cb0c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="0cb0c-108">Pentru mai multe informații, consultați [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="0cb0c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
