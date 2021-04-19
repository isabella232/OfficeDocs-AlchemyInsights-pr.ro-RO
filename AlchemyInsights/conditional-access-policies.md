---
title: Politici de acces condițional
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817292"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="db805-102">Politici de acces condițional</span><span class="sxs-lookup"><span data-stu-id="db805-102">Conditional Access policies</span></span>

<span data-ttu-id="db805-103">Accesul condițional este o capacitate a Azure AD care vă permite să impuneți controale asupra accesului la aplicațiile din mediul dvs., toate acestea bazate pe condiții specifice și gestionate dintr-o locație centrală.</span><span class="sxs-lookup"><span data-stu-id="db805-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="db805-104">Aflați mai multe despre [Accesul condițional Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="db805-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="db805-105">**Notă**: Dacă entitatea dvs. găzduită a fost creată după 21 octombrie 2019 și vi se solicită în mod neașteptat pentru MFA, probabil că aveți [setările implicite de securitate](https://aka.ms/securitydefaults) activate în entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="db805-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="db805-106">**Pentru a Gestiona setările implicite de securitate**</span><span class="sxs-lookup"><span data-stu-id="db805-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="db805-107">Conectați-vă la [centrul de administrare](https://go.microsoft.com/fwlink/p/?linkid=834822) utilizând acreditările de administrator Global.</span><span class="sxs-lookup"><span data-stu-id="db805-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="db805-108">Accesați [Proprietăți Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="db805-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="db805-109">În partea de jos a paginii, faceți clic pe **Gestionați Valorile Implicite de Securitate**.</span><span class="sxs-lookup"><span data-stu-id="db805-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="db805-110">Faceți clic pe **Da** pentru a activa setările implicite de securitate sau pe **Nu** pentru a dezactiva setările implicite de securitate.</span><span class="sxs-lookup"><span data-stu-id="db805-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
