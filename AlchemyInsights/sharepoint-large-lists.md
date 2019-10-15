---
title: Liste mari SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488529"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="c721d-102">Lucrați cu liste mari și biblioteci în SharePoint</span><span class="sxs-lookup"><span data-stu-id="c721d-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="c721d-103">Listele și bibliotecile SharePoint pot conține până la 30.000.000 de elemente, dar când au mai mult de 5.000 de articole, este posibil să vedeți o eroare prag Vizualizare listă atunci când încercați să lucrați cu ele.</span><span class="sxs-lookup"><span data-stu-id="c721d-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="c721d-104">Acest prag este în vigoare pentru a menține performanța serviciului.</span><span class="sxs-lookup"><span data-stu-id="c721d-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="c721d-105">Nu poate fi schimbată.</span><span class="sxs-lookup"><span data-stu-id="c721d-105">It can't be changed.</span></span> <span data-ttu-id="c721d-106">Pentru a evita lovirea acestui prag:</span><span class="sxs-lookup"><span data-stu-id="c721d-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="c721d-107">**Utilizarea modernă**</span><span class="sxs-lookup"><span data-stu-id="c721d-107">**Use modern**</span></span>

<span data-ttu-id="c721d-108">Vizualizări care arată multe elemente de lucru cel mai bine în experiența modernă.</span><span class="sxs-lookup"><span data-stu-id="c721d-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="c721d-109">[Folosește experiența modernă](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) pentru a evita erorile pe care le-ai putea vedea în experiența clasică.</span><span class="sxs-lookup"><span data-stu-id="c721d-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="c721d-110">**Adăugare indexuri**</span><span class="sxs-lookup"><span data-stu-id="c721d-110">**Add indexes**</span></span>

<span data-ttu-id="c721d-111">Când filtrați sau sortați după o coloană care nu are un index, este posibil să vedeți un mesaj de eroare.</span><span class="sxs-lookup"><span data-stu-id="c721d-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="c721d-112">[Adăugați manual un index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) din **Setări listă** în meniul de setări, apoi **coloane indexate**.</span><span class="sxs-lookup"><span data-stu-id="c721d-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="c721d-113">**Editarea vizualizării listei**</span><span class="sxs-lookup"><span data-stu-id="c721d-113">**Edit the list view**</span></span>

<span data-ttu-id="c721d-114">Dacă apare o eroare atunci când lucrați cu o listă mare, [editați vizualizarea listei](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="c721d-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="c721d-115">Următoarele patru modificări vor elimina erorile de prag de vizualizare listă.</span><span class="sxs-lookup"><span data-stu-id="c721d-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="c721d-116">Efectuați toate cele patru modificări pentru a elimina toate erorile.</span><span class="sxs-lookup"><span data-stu-id="c721d-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="c721d-117">Dacă încă mai primești erori, verifică [gestionarea listelor mari și a bibliotecilor](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="c721d-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="c721d-118">Selectați **niciuna** de la **cel mai bun fel după coloană** și **apoi sortați după coloană**.</span><span class="sxs-lookup"><span data-stu-id="c721d-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="c721d-119">Selectați **niciuna** din ambele **grupe în primul rând după coloană** , **apoi grupați după coloană**.</span><span class="sxs-lookup"><span data-stu-id="c721d-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="c721d-120">Selectați **niciuna** pentru toate coloanele din secțiunea **totaluri** .</span><span class="sxs-lookup"><span data-stu-id="c721d-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="c721d-121">Deselectați toate, dar o coloană pentru afișare din secțiunea **coloane** .</span><span class="sxs-lookup"><span data-stu-id="c721d-121">Deselect all but one column for display from the **Columns** section.</span></span>

