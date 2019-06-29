---
title: Actualizarea serverelor de nume de domeniu la Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 8e25c510233f2a00d133ea69a338141c5a475465
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352901"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e04a0-102">Actualizarea serverelor de nume de domeniu la Office 365</span><span class="sxs-lookup"><span data-stu-id="e04a0-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e04a0-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="e04a0-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e04a0-104">Pentru a vă configura domeniul în Office 365, serverele de nume de la registratorul dvs. trebuie actualizate.</span><span class="sxs-lookup"><span data-stu-id="e04a0-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="e04a0-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="e04a0-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e04a0-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="e04a0-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="e04a0-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="e04a0-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e04a0-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e04a0-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e04a0-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e04a0-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e04a0-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="e04a0-110">Save changes.</span></span>

<span data-ttu-id="e04a0-111">Puteți găsi instrucțiuni detaliate și în acest articol: [Modificarea serverelor de nume pentru a configura Office 365 cu orice registrator de domeniu](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="e04a0-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  