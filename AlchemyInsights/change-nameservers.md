---
title: Modificarea serverelor de nume
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902941"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="77511-102">Actualizarea serverelor de nume de domeniu la Office 365</span><span class="sxs-lookup"><span data-stu-id="77511-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="77511-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="77511-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="77511-104">Pentru a vă configura domeniul în Office 365, serverele de nume de la registratorul dvs. trebuie actualizate.</span><span class="sxs-lookup"><span data-stu-id="77511-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="77511-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="77511-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="77511-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="77511-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="77511-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="77511-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="77511-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="77511-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="77511-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="77511-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="77511-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="77511-110">Save changes.</span></span>

<span data-ttu-id="77511-111">Puteți găsi instrucțiuni detaliate și în acest articol: [Modificarea serverelor de nume pentru a configura Office 365 cu orice registrator de domeniu](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="77511-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  