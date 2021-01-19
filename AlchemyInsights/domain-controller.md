---
title: Controler de domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901311"
---
# <a name="domain-controller"></a><span data-ttu-id="ece05-102">Controler de domeniu</span><span class="sxs-lookup"><span data-stu-id="ece05-102">Domain controller</span></span>

<span data-ttu-id="ece05-103">**Nu reușiți să activați AAD-DS sau implementarea nu reușește**</span><span class="sxs-lookup"><span data-stu-id="ece05-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="ece05-104">Pentru a rezolva problema serviciului de domeniu Azure AD (AAD-DS) care nu este activat sau nu este implementat, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="ece05-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="ece05-105">Dacă utilizați o rețea virtuală deja existentă, Verificați-vă NSG pentru reguli care blochează porturile necesare pentru a se sincroniza în AAD-DS în portal https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="ece05-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="ece05-106">Verificați dacă mesajul de eroare este răspuns în acest ghid de depanare disponibil în  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="ece05-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="ece05-107">Încercați să implementați servicii de domeniu Azure AD într-o rețea virtuală nouă.</span><span class="sxs-lookup"><span data-stu-id="ece05-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="ece05-108">Urmați ghidul introductiv despre cum să implementați AAD-DS, disponibil la [tutorial pentru a crea servicii de domeniu AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="ece05-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="ece05-109">Dacă întâmpinați probleme cu implementarea serviciilor de domeniu Azure AD, consultați [Depanarea serviciilor de domeniu AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pentru a rezolva erorile comune, pentru a vă ajuta să lucrați din nou.</span><span class="sxs-lookup"><span data-stu-id="ece05-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="ece05-110">**Nu se poate dezactiva AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="ece05-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="ece05-111">AAD-DS nu poate fi în pauză.</span><span class="sxs-lookup"><span data-stu-id="ece05-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="ece05-112">Dacă doriți să opriți utilizarea domeniului gestionat, acesta trebuie șters.</span><span class="sxs-lookup"><span data-stu-id="ece05-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="ece05-113">Dacă întâmpinați probleme, pentru a rezolva mesaje de eroare comune și pentru pașii de depanare asociați, pentru a vă ajuta să începeți lucrul, consultați [Depanarea serviciilor de domeniu Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="ece05-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
