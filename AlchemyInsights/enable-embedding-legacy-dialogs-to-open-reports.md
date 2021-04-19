---
title: Activarea încorporării casetelor de dialog moștenite pentru a deschide rapoarte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814276"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="09ff0-102">Activarea încorporării casetelor de dialog moștenite pentru a deschide rapoarte</span><span class="sxs-lookup"><span data-stu-id="09ff0-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="09ff0-103">**Simptom**</span><span class="sxs-lookup"><span data-stu-id="09ff0-103">**Symptom**</span></span>

<span data-ttu-id="09ff0-104">Utilizatorii nu pot deschide rapoarte.</span><span class="sxs-lookup"><span data-stu-id="09ff0-104">Users are unable to open reports.</span></span> <span data-ttu-id="09ff0-105">"Ceva nu a mers bine.</span><span class="sxs-lookup"><span data-stu-id="09ff0-105">"Something has gone wrong.</span></span> <span data-ttu-id="09ff0-106">Consultați detaliile tehnice pentru mai multe detalii."</span><span class="sxs-lookup"><span data-stu-id="09ff0-106">Check technical details for more details."</span></span>

<span data-ttu-id="09ff0-107">**Cauză**</span><span class="sxs-lookup"><span data-stu-id="09ff0-107">**Cause**</span></span>

<span data-ttu-id="09ff0-108">Rapoartele nu reușesc să fie încărcate în INS cu eroarea "descriptorul de formulare este nul sau nu este definit".</span><span class="sxs-lookup"><span data-stu-id="09ff0-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="09ff0-109">Rapoartele din CASETELE DE DIALOG necesită în continuare casete de dialog moștenite, prin urmare, sistemul clientului trebuie să aibă activată opțiunea *DelegacyDialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="09ff0-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="09ff0-110">**Soluție**</span><span class="sxs-lookup"><span data-stu-id="09ff0-110">**Solution**</span></span>

1. <span data-ttu-id="09ff0-111">Accesați Setări **>Administrare > System Settings (Setări > fila General).**</span><span class="sxs-lookup"><span data-stu-id="09ff0-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="09ff0-112">Setați "Activați încorporarea anumitor casete de dialog moștenite în clientul browser Interfață unificată" la **Da**.</span><span class="sxs-lookup"><span data-stu-id="09ff0-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
