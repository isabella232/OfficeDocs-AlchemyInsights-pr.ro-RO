---
title: Actualizați serverele de nume de domeniu pentru a indica spre Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720005"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="db038-102">Actualizați serverele de nume de domeniu pentru a indica spre Microsoft</span><span class="sxs-lookup"><span data-stu-id="db038-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="db038-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="db038-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="db038-104">Pentru a configura domeniul cu Microsoft, serverele de nume de la registrator trebuie să fie actualizate.</span><span class="sxs-lookup"><span data-stu-id="db038-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="db038-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="db038-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="db038-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="db038-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="db038-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="db038-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="db038-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="db038-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="db038-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="db038-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="db038-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="db038-110">Save changes.</span></span>

<span data-ttu-id="db038-111">De asemenea, puteți găsi instrucțiuni detaliate în acest articol: [Modificați serverele de nume pentru a configura Microsoft 365 cu orice registrator de domeniu](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="db038-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  