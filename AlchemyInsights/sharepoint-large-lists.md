---
title: Liste mari SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720145"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="66e06-102">Lucrul cu liste și biblioteci mari în SharePoint</span><span class="sxs-lookup"><span data-stu-id="66e06-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="66e06-103">Listele și bibliotecile SharePoint pot conține până la 30.000.000 de elemente, dar atunci când au mai mult de 5.000 de elemente, este posibil să vedeți o eroare de prag a vizualizării listă atunci când încercați să lucrați cu ele.</span><span class="sxs-lookup"><span data-stu-id="66e06-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="66e06-104">Acest prag există pentru a menține performanța serviciului.</span><span class="sxs-lookup"><span data-stu-id="66e06-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="66e06-105">Acesta nu poate fi modificat.</span><span class="sxs-lookup"><span data-stu-id="66e06-105">It can't be changed.</span></span> <span data-ttu-id="66e06-106">Pentru a evita atingerea acestui prag:</span><span class="sxs-lookup"><span data-stu-id="66e06-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="66e06-107">**Utilizați modern**</span><span class="sxs-lookup"><span data-stu-id="66e06-107">**Use modern**</span></span>

<span data-ttu-id="66e06-108">Vizualizările care afișează cele mai bune elemente funcționează cel mai bine în experiența modernă.</span><span class="sxs-lookup"><span data-stu-id="66e06-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="66e06-109">[Utilizați experiența modernă](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) pentru a evita erorile pe care le-ați putea vedea în experiența clasică.</span><span class="sxs-lookup"><span data-stu-id="66e06-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="66e06-110">**Adăugarea indexurilor**</span><span class="sxs-lookup"><span data-stu-id="66e06-110">**Add indexes**</span></span>

<span data-ttu-id="66e06-111">Atunci când filtrați sau sortați după o coloană care nu are un index, este posibil să vedeți un mesaj de eroare.</span><span class="sxs-lookup"><span data-stu-id="66e06-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="66e06-112">[Adăugați manual un index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) din **Setări listă** din meniul Setări, apoi **coloane indexate**.</span><span class="sxs-lookup"><span data-stu-id="66e06-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="66e06-113">**Editarea vizualizării listă**</span><span class="sxs-lookup"><span data-stu-id="66e06-113">**Edit the list view**</span></span>

<span data-ttu-id="66e06-114">Dacă apare o eroare atunci când lucrați cu o listă mare, [editați vizualizarea listă](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="66e06-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="66e06-115">Următoarele patru modificări vor elimina erorile de prag pentru vizualizarea listă.</span><span class="sxs-lookup"><span data-stu-id="66e06-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="66e06-116">Efectuați toate cele patru modificări pentru a elimina toate erorile.</span><span class="sxs-lookup"><span data-stu-id="66e06-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="66e06-117">Dacă primiți în continuare erori, verificați [gestionarea listelor și bibliotecilor mari](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="66e06-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="66e06-118">Selectați **fără** din ambele **Sortare după coloană** , **apoi sortați după coloană**.</span><span class="sxs-lookup"><span data-stu-id="66e06-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="66e06-119">Selectați **fără** din **primul grup după coloană** , **apoi grupați după coloană**.</span><span class="sxs-lookup"><span data-stu-id="66e06-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="66e06-120">Selectați **fără** pentru toate coloanele din secțiunea **totaluri** .</span><span class="sxs-lookup"><span data-stu-id="66e06-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="66e06-121">Deselectați toate, dar o coloană pentru afișare din secțiunea **coloane** .</span><span class="sxs-lookup"><span data-stu-id="66e06-121">Deselect all but one column for display from the **Columns** section.</span></span>

