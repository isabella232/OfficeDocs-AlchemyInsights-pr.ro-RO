---
title: Liste mari SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767297"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="9bc50-102">Lucrul cu liste și biblioteci mari în SharePoint</span><span class="sxs-lookup"><span data-stu-id="9bc50-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="9bc50-103">Listele și bibliotecile SharePoint pot conține până la 30 de milioane de elemente, dar atunci când au mai mult de 5.000 de elemente, este posibil să vedeți o eroare Prag vizualizare listă atunci când încercați să lucrați cu acestea.</span><span class="sxs-lookup"><span data-stu-id="9bc50-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="9bc50-104">Acest prag există pentru a menține performanța serviciului.</span><span class="sxs-lookup"><span data-stu-id="9bc50-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="9bc50-105">Acesta nu poate fi modificat.</span><span class="sxs-lookup"><span data-stu-id="9bc50-105">It can't be changed.</span></span> <span data-ttu-id="9bc50-106">Pentru a evita atingerea acestui prag:</span><span class="sxs-lookup"><span data-stu-id="9bc50-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="9bc50-107">**Utilizarea modernă**</span><span class="sxs-lookup"><span data-stu-id="9bc50-107">**Use modern**</span></span>

<span data-ttu-id="9bc50-108">Opiniile care arată multe elemente funcționează cel mai bine în experiența modernă.</span><span class="sxs-lookup"><span data-stu-id="9bc50-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="9bc50-109">[Utilizați experiența modernă](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) pentru a evita erorile pe care le-ați putea vedea în experiența clasică.</span><span class="sxs-lookup"><span data-stu-id="9bc50-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="9bc50-110">**Adăugarea indexurilor**</span><span class="sxs-lookup"><span data-stu-id="9bc50-110">**Add indexes**</span></span>

<span data-ttu-id="9bc50-111">Când filtrați sau sortați după o coloană care nu are un index, este posibil să vedeți un mesaj de eroare.</span><span class="sxs-lookup"><span data-stu-id="9bc50-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="9bc50-112">[Adăugați](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manual un index din **Setări listă** din meniul de setări, apoi **Coloane indexate**.</span><span class="sxs-lookup"><span data-stu-id="9bc50-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="9bc50-113">**Editarea vizualizării listă**</span><span class="sxs-lookup"><span data-stu-id="9bc50-113">**Edit the list view**</span></span>

<span data-ttu-id="9bc50-114">Dacă apare o eroare atunci când lucrați cu o listă mare, [editați vizualizarea listă](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="9bc50-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="9bc50-115">Următoarele patru modificări vor elimina erorile de prag de vizualizare listă.</span><span class="sxs-lookup"><span data-stu-id="9bc50-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="9bc50-116">Efectuați toate cele patru modificări pentru a elimina toate erorile.</span><span class="sxs-lookup"><span data-stu-id="9bc50-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="9bc50-117">Dacă primiți în continuare erori, consultați [Gestionareliste și biblioteci mari](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="9bc50-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="9bc50-118">Selectați **Nici unul** din **ambele prima sortare după coloană** și **apoi sortați după coloană**.</span><span class="sxs-lookup"><span data-stu-id="9bc50-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="9bc50-119">Selectați **Niciuna** din ambele **primul grup după coloană** și **Apoi grupați după coloană**.</span><span class="sxs-lookup"><span data-stu-id="9bc50-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="9bc50-120">Selectați **Niciuna** pentru toate coloanele din secțiunea **Totaluri.**</span><span class="sxs-lookup"><span data-stu-id="9bc50-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="9bc50-121">Deselectați toate coloanele, cu excepția unei coloane, pentru afișare din secțiunea **Coloane.**</span><span class="sxs-lookup"><span data-stu-id="9bc50-121">Deselect all but one column for display from the **Columns** section.</span></span>

