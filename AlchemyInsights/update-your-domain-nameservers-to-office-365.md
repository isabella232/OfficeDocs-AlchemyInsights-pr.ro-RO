---
title: Actualizarea serverelor de nume de domeniu pentru a indica la Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734923"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="1be54-102">Actualizarea serverelor de nume de domeniu pentru a indica la Microsoft</span><span class="sxs-lookup"><span data-stu-id="1be54-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="1be54-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="1be54-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="1be54-104">Pentru a vă configura domeniul cu Microsoft, trebuie să actualizați serverele de nume de la registrator.</span><span class="sxs-lookup"><span data-stu-id="1be54-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="1be54-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="1be54-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="1be54-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="1be54-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="1be54-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="1be54-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="1be54-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1be54-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="1be54-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1be54-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="1be54-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="1be54-110">Save changes.</span></span>

<span data-ttu-id="1be54-111">De asemenea, puteți găsi instrucțiuni detaliate în acest articol: modificarea serverelor [de nume pentru a configura Microsoft 365 cu orice registrator de domeniu](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="1be54-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  