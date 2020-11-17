---
title: Rol privilegiat de gestionare a identității
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089154"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="89ed1-102">Rolul de gestionare a identității privilegiat (PIM)</span><span class="sxs-lookup"><span data-stu-id="89ed1-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="89ed1-103">**Permisiunile nu se acordă după activarea unui rol**</span><span class="sxs-lookup"><span data-stu-id="89ed1-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="89ed1-104">Atunci când activați un rol în Azure AD privilegiat Identity Management (PIM), activarea poate să nu se propage instantaneu la toate portaluri care necesită rolul privilegiat.</span><span class="sxs-lookup"><span data-stu-id="89ed1-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="89ed1-105">Uneori, chiar dacă modificarea este propagată, memorarea în cache Web într-un portal poate avea ca rezultat modificarea care nu intră în vigoare imediat.</span><span class="sxs-lookup"><span data-stu-id="89ed1-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="89ed1-106">Dacă activarea este întârziată, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="89ed1-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="89ed1-107">Deconectați-vă de la portalul Azure, apoi conectați-vă din nou.</span><span class="sxs-lookup"><span data-stu-id="89ed1-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="89ed1-108">Atunci când activați un rol Azure AD sau un rol de resurse Azure, veți vedea etapele de activare.</span><span class="sxs-lookup"><span data-stu-id="89ed1-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="89ed1-109">După ce se termină toate etapele, veți vedea un link "deconectare".</span><span class="sxs-lookup"><span data-stu-id="89ed1-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="89ed1-110">Puteți utiliza acest link pentru a vă deconecta. Acest lucru va rezolva majoritatea cazurilor pentru întârzierea activării.</span><span class="sxs-lookup"><span data-stu-id="89ed1-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="89ed1-111">În PIM, asigurați-vă că sunteți listat ca membru al rolului.</span><span class="sxs-lookup"><span data-stu-id="89ed1-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="89ed1-112">Dacă activați rolul de administrator Exchange, asigurați-vă că vă deconectați și vă conectați din nou.</span><span class="sxs-lookup"><span data-stu-id="89ed1-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="89ed1-113">Dacă problema persistă, deschideți un tichet de asistență și creșteți-l ca problemă.</span><span class="sxs-lookup"><span data-stu-id="89ed1-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="89ed1-114">Dacă utilizați rolul de administrator Exchange pentru a accesa centrul de securitate și conformitate, consultați Pasul următor.</span><span class="sxs-lookup"><span data-stu-id="89ed1-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="89ed1-115">Dacă activați un rol pentru a accesa centrul de securitate și conformitate sau dacă activați rolul de administrator SharePoint, veți avea câteva întârzieri de activare de la câteva minute până la câteva ore.</span><span class="sxs-lookup"><span data-stu-id="89ed1-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="89ed1-116">Aceasta este o problemă cunoscută și lucrăm în mod activ cu aceste echipe pentru a rezolva această problemă cât mai curând posibil.</span><span class="sxs-lookup"><span data-stu-id="89ed1-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="89ed1-117">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="89ed1-117">For more information, see:</span></span>

- [<span data-ttu-id="89ed1-118">Activarea rolurilor de publicitate Azure în PIM</span><span class="sxs-lookup"><span data-stu-id="89ed1-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="89ed1-119">Activarea rolurilor de resurse Azure în PIM</span><span class="sxs-lookup"><span data-stu-id="89ed1-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="89ed1-120">**Permisiunile nu sunt eliminate după ce dezactivarea unui rol sau activarea rolului expiră**</span><span class="sxs-lookup"><span data-stu-id="89ed1-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="89ed1-121">Atunci când dezactivați un rol în managementul de identitate privilegiat din Azure AD sau când expiră o perioadă de activare a rolului, poate exista o întârziere în care continuați să aveți acces.</span><span class="sxs-lookup"><span data-stu-id="89ed1-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="89ed1-122">Dacă dezactivarea este întârziată, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="89ed1-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="89ed1-123">Dacă deactivați rolul de administrator Exchange sau perioada de activare a rolului expiră și observați o întârziere semnificativă înainte ca permisiunile să fie eliminate, deschideți un tichet de asistență și spuneți-i inginerului de asistență să vă ajute să faceți un bilet cu echipa de gestionare a accesului privilegiat (PAM) în Office despre această problemă.</span><span class="sxs-lookup"><span data-stu-id="89ed1-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="89ed1-124">Dacă perioada de activare a expirat, dar încă aveți sesiunea de browser deschisă, închideți browserul.</span><span class="sxs-lookup"><span data-stu-id="89ed1-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="89ed1-125">Puteți continua să utilizați rolul până când închideți acea sesiune.</span><span class="sxs-lookup"><span data-stu-id="89ed1-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="89ed1-126">Aceasta este o problemă cunoscută și ne uităm la o remediere potențială pentru a revoca în mod activ fiecare sesiune după ce activarea a expirat.</span><span class="sxs-lookup"><span data-stu-id="89ed1-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="89ed1-127">Dacă întârzierea dumneavoastră este diferită de aceste două scenarii, vă rugăm să deschideți un tichet de asistență.</span><span class="sxs-lookup"><span data-stu-id="89ed1-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
