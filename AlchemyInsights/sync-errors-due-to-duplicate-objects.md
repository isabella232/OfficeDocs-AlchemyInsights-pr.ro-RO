---
title: 902 (erorile de sincronizare din cauza obiectelor dublate)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737353"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="3661f-102">Erorile de sincronizare din cauza obiectelor dublate</span><span class="sxs-lookup"><span data-stu-id="3661f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="3661f-103">Este posibil să primiți unul dintre următoarele mesaje de eroare atunci când se termină sincronizarea directorului în Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="3661f-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="3661f-104">Nu se poate actualiza acest obiect în Microsoft Online Services, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din directorul local.</span><span class="sxs-lookup"><span data-stu-id="3661f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="3661f-105">Un obiect sincronizat cu aceeași adresă proxy există deja în directorul Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="3661f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="3661f-106">Nu se poate actualiza acest obiect, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din serviciile directorului local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3661f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="3661f-107">Pentru a identifica și a remedia problema, descărcați și derulează [Instrumentul de remediere a erorilor IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="3661f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="3661f-108">Pentru mai multe informații, consultați [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="3661f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
