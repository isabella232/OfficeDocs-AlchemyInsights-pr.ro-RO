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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708074"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="24e44-102">Erorile de sincronizare din cauza obiectelor dublate</span><span class="sxs-lookup"><span data-stu-id="24e44-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="24e44-103">Este posibil să primiți unul dintre următoarele mesaje de eroare atunci când se termină sincronizarea directorului în Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="24e44-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="24e44-104">Nu se poate actualiza acest obiect în Microsoft Online Services, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din directorul local.</span><span class="sxs-lookup"><span data-stu-id="24e44-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="24e44-105">Un obiect sincronizat cu aceeași adresă proxy există deja în directorul Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="24e44-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="24e44-106">Nu se poate actualiza acest obiect, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din serviciile directorului local: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="24e44-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="24e44-107">Pentru a identifica și a remedia problema, descărcați și derulează [Instrumentul de remediere a erorilor IdFix DirSync](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="24e44-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="24e44-108">Pentru mai multe informații, consultați [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="24e44-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
