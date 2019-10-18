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
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736661"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e4b5a-102">Actualizarea serverelor de nume de domeniu la Office 365</span><span class="sxs-lookup"><span data-stu-id="e4b5a-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e4b5a-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="e4b5a-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e4b5a-104">Pentru a vă configura domeniul în Office 365, serverele de nume de la registratorul dvs. trebuie actualizate.</span><span class="sxs-lookup"><span data-stu-id="e4b5a-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="e4b5a-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="e4b5a-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e4b5a-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="e4b5a-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="e4b5a-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="e4b5a-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e4b5a-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e4b5a-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e4b5a-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e4b5a-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e4b5a-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="e4b5a-110">Save changes.</span></span>

<span data-ttu-id="e4b5a-111">Puteți găsi instrucțiuni detaliate și în acest articol: [Modificarea serverelor de nume pentru a configura Office 365 cu orice registrator de domeniu](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="e4b5a-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  