---
title: Modificarea serverelor de nume
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706767"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="5e540-102">Actualizarea serverelor de nume de domeniu pentru a indica la Microsoft</span><span class="sxs-lookup"><span data-stu-id="5e540-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="5e540-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="5e540-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5e540-104">Pentru a vă configura domeniul în Microsoft 365, serverele de nume de la registratorul dvs. trebuie actualizate.</span><span class="sxs-lookup"><span data-stu-id="5e540-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="5e540-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="5e540-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5e540-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="5e540-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="5e540-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="5e540-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="5e540-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5e540-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="5e540-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5e540-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="5e540-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="5e540-110">Save changes.</span></span>

<span data-ttu-id="5e540-111">Puteți găsi instrucțiuni detaliate și în acest articol: [Modificarea serverelor de nume cu orice registrator de domeniu](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="5e540-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  