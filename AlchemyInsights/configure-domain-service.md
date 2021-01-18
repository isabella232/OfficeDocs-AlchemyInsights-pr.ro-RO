---
title: Configurarea serviciului de domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885690"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="5479e-102">Nu reușiți să activați AAD-DS sau implementarea nu reușește</span><span class="sxs-lookup"><span data-stu-id="5479e-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="5479e-103">Pentru a rezolva problema serviciului de domeniu Azure AD (AAD-DS) care nu este activat sau nu este implementat, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="5479e-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="5479e-104">Dacă utilizați o rețea virtuală deja existentă, Verificați-vă NSG pentru reguli care blochează porturile necesare pentru a se sincroniza în AAD-DS în portal https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="5479e-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="5479e-105">Verificați dacă mesajul de eroare este răspuns în acest ghid de depanare disponibil în  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="5479e-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="5479e-106">Încercați să implementați servicii de domeniu Azure AD într-o rețea virtuală nouă.</span><span class="sxs-lookup"><span data-stu-id="5479e-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="5479e-107">Urmați ghidul introductiv despre cum să implementați AAD-DS: [crearea și configurarea serviciilor de domeniu AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="5479e-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="5479e-108">Dacă întâmpinați probleme cu implementarea serviciilor de domeniu Azure AD, consultați [Depanarea serviciilor de domeniu AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pentru a rezolva erorile comune, pentru a vă ajuta să lucrați din nou.</span><span class="sxs-lookup"><span data-stu-id="5479e-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="5479e-109">**Nu se poate dezactiva AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="5479e-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="5479e-110">AAD-DS nu poate fi în pauză.</span><span class="sxs-lookup"><span data-stu-id="5479e-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="5479e-111">Dacă doriți să opriți utilizarea domeniului gestionat, acesta trebuie șters.</span><span class="sxs-lookup"><span data-stu-id="5479e-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="5479e-112">Pentru a șterge domeniul gestionat, consultați [ștergerea serviciului de domeniu AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="5479e-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



