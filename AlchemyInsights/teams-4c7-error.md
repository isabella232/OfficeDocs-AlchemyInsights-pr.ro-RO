---
title: Eroare Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786681"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="74db9-102">Eroare 4c7 în Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="74db9-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="74db9-103">Această eroare apare deoarece Microsoft Teams necesită autentificarea Forms.</span><span class="sxs-lookup"><span data-stu-id="74db9-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="74db9-104">Când implementați Active Directory Federation Services (AD FS), autentificarea Formulare nu este activată în mod implicit pentru intranet.</span><span class="sxs-lookup"><span data-stu-id="74db9-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="74db9-105">Dacă autentificarea integrată Windows nu reușește, vi se solicită să vă conectați utilizând autentificarea Forms.</span><span class="sxs-lookup"><span data-stu-id="74db9-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="74db9-106">Pentru a rezolva această problemă, activați autentificarea Forms utilizând utilitarul de completare snap-in AD FS Microsoft Management Console (MMC) pe computerul care are copia locală de Active Directory.</span><span class="sxs-lookup"><span data-stu-id="74db9-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="74db9-107">Pentru a proceda astfel, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="74db9-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="74db9-108">În panoul de navigare, navigați **la Politici de autentificare**.</span><span class="sxs-lookup"><span data-stu-id="74db9-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="74db9-109">Sub **Acțiuni,** în panoul de detalii, **selectați Editare autentificare primară globală.**</span><span class="sxs-lookup"><span data-stu-id="74db9-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="74db9-110">Pe fila **Intranet,** selectați **Autentificare formulare.**</span><span class="sxs-lookup"><span data-stu-id="74db9-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="74db9-111">Selectați **OK** (sau **Se aplică**).</span><span class="sxs-lookup"><span data-stu-id="74db9-111">Select **OK** (or **Apply**).</span></span>