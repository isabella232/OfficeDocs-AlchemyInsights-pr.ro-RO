---
title: Echipele 4C 7 eroare
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796312"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="f6325-102">eroare 4C 7 în Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="f6325-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="f6325-103">Această eroare apare deoarece Microsoft teams necesită autentificarea formularelor.</span><span class="sxs-lookup"><span data-stu-id="f6325-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="f6325-104">Când implementați consolidare servicii de federalizare Active Directory (AD FS), autentificarea formularelor nu este activată pentru intranet în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="f6325-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="f6325-105">Dacă autentificarea integrată Windows nu reușește, vi se solicită să faceți sign in utilizând autentificarea formularelor.</span><span class="sxs-lookup"><span data-stu-id="f6325-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="f6325-106">Pentru a rezolva această problemă, activați autentificarea formularelor utilizând utilitarul de completare snap-in AD FS Microsoft Management Console (MMC) pe computerul care are copia locală a Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f6325-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="f6325-107">Pentru a proceda astfel, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="f6325-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="f6325-108">În panoul de navigare, răsfoiți la **politicile de autentificare**.</span><span class="sxs-lookup"><span data-stu-id="f6325-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="f6325-109">Sub **acțiuni** în panoul de detalii, selectați **editați autentificarea primară globală**.</span><span class="sxs-lookup"><span data-stu-id="f6325-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="f6325-110">În fila **intranet** , selectați **autentificarea formularelor**.</span><span class="sxs-lookup"><span data-stu-id="f6325-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="f6325-111">Selectați **OK** (sau **aplicați**).</span><span class="sxs-lookup"><span data-stu-id="f6325-111">Select **OK** (or **Apply**).</span></span>