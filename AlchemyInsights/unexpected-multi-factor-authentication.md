---
title: Autentificare multi-factor neașteptată
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946734"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="2eb2e-102">Autentificare multi-factor neașteptată</span><span class="sxs-lookup"><span data-stu-id="2eb2e-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="2eb2e-103">Dacă entitatea dvs. găzduită a fost creată după 21 octombrie 2019 și vi se solicită în mod neașteptat pentru MFA, probabil că aveți [setările implicite de securitate](http://aka.ms/securitydefaults) activate în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="2eb2e-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="2eb2e-104">Pentru a Gestiona setările implicite de securitate:</span><span class="sxs-lookup"><span data-stu-id="2eb2e-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="2eb2e-105">Conectați-vă la [centrul de administrare](https://go.microsoft.com/fwlink/p/?linkid=834822) utilizând acreditările de administrator Global.</span><span class="sxs-lookup"><span data-stu-id="2eb2e-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="2eb2e-106">Accesați [Proprietăți Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="2eb2e-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="2eb2e-107">În partea de jos a paginii, faceți clic pe **Gestionați Valorile Implicite de Securitate**.</span><span class="sxs-lookup"><span data-stu-id="2eb2e-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="2eb2e-108">Faceți clic pe **Da** pentru a activa setările implicite de securitate și **Nu** pentru a dezactiva setările implicite de securitate.</span><span class="sxs-lookup"><span data-stu-id="2eb2e-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
