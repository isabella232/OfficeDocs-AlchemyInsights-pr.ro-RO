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
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 148fbee1c14a8da6ede5ec5ccae90b1a4340ce32
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363089"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="f749e-102">Actualizarea serverelor de nume de domeniu la Office 365</span><span class="sxs-lookup"><span data-stu-id="f749e-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="f749e-103">Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.</span><span class="sxs-lookup"><span data-stu-id="f749e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="f749e-104">Pentru a vă configura domeniul în Office 365, serverele de nume de la registratorul dvs. trebuie actualizate.</span><span class="sxs-lookup"><span data-stu-id="f749e-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="f749e-105">Creați sau editați înregistrările serverului de nume în registratorul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="f749e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="f749e-106">Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.</span><span class="sxs-lookup"><span data-stu-id="f749e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="f749e-107">Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:</span><span class="sxs-lookup"><span data-stu-id="f749e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="f749e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f749e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="f749e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f749e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="f749e-110">Salvați modificările.</span><span class="sxs-lookup"><span data-stu-id="f749e-110">Save changes.</span></span>

<span data-ttu-id="f749e-111">Puteți găsi instrucțiuni detaliate și în acest articol: [Modificarea serverelor de nume pentru a configura Office 365 cu orice registrator de domeniu](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="f749e-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  