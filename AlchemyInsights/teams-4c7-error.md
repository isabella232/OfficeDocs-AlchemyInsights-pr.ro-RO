---
title: Eroare 4c7 teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700215"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="d6394-102">eroare 4c7 în Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="d6394-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="d6394-103">Această eroare apare deoarece Microsoft teams necesită autentificarea formularelor.</span><span class="sxs-lookup"><span data-stu-id="d6394-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="d6394-104">Atunci când implementați Active Directory Federation Services (AD FS), autentificarea de formulare nu este activată implicit pentru intranet.</span><span class="sxs-lookup"><span data-stu-id="d6394-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="d6394-105">Dacă autentificarea integrată Windows nu reușește, vi se solicită să vă conectați utilizând autentificarea formularelor.</span><span class="sxs-lookup"><span data-stu-id="d6394-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="d6394-106">Pentru a rezolva această problemă, activați autentificarea formularelor utilizând utilitarul de completare snap-in AD FS Microsoft consolă de gestionare (MMC) pe computerul care conține copia locală a Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6394-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="d6394-107">Pentru a proceda astfel, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="d6394-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="d6394-108">În panoul de navigare, răsfoiți la **politicile de autentificare**.</span><span class="sxs-lookup"><span data-stu-id="d6394-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="d6394-109">Sub **acțiuni** în panoul de detalii, selectați **Editare autentificare principală globală**.</span><span class="sxs-lookup"><span data-stu-id="d6394-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="d6394-110">Pe fila **intranet** , selectați **autentificare formulare**.</span><span class="sxs-lookup"><span data-stu-id="d6394-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="d6394-111">Selectați **OK** (sau **aplicați**).</span><span class="sxs-lookup"><span data-stu-id="d6394-111">Select **OK** (or **Apply**).</span></span>