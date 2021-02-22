---
title: Ascunderea folderelor publice
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315437"
---
# <a name="hide-public-folders"></a><span data-ttu-id="29a90-102">Ascunderea folderelor publice</span><span class="sxs-lookup"><span data-stu-id="29a90-102">Hide public folders</span></span>

<span data-ttu-id="29a90-103">**Pentru a ascunde întregul arbore de foldere publice**:</span><span class="sxs-lookup"><span data-stu-id="29a90-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="29a90-104">Utilizați pașii din [acest](https://aka.ms/ControlPF) articol pentru a ascunde întregul arbore de foldere publice de la selectiv sau de la toți utilizatorii.</span><span class="sxs-lookup"><span data-stu-id="29a90-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="29a90-105">**Pentru a ascunde un anumit folder public**:</span><span class="sxs-lookup"><span data-stu-id="29a90-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="29a90-106">Adăugarea de permisiuni pentru utilizatorii care trebuie să acceseze folderul public</span><span class="sxs-lookup"><span data-stu-id="29a90-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="29a90-107">Eliminați **implicit** utilizatorul din lista de **permisiuni** :</span><span class="sxs-lookup"><span data-stu-id="29a90-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
