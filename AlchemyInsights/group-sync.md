---
title: Sincronizare grup
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256788"
---
# <a name="group-sync"></a><span data-ttu-id="ce99f-102">Sincronizare grup</span><span class="sxs-lookup"><span data-stu-id="ce99f-102">Group sync</span></span>

<span data-ttu-id="ce99f-103">Acest articol oferă instrucțiuni despre sincronizarea grupurilor.</span><span class="sxs-lookup"><span data-stu-id="ce99f-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="ce99f-104">Dacă un administrator global sau un proprietar de grup nu poate modifica proprietățile de grup sau adăuga membri sau atribui proprietarilor din portalul Azure, asigurați-vă că sursa autorității pentru grup este Azure Active Directory (Azure AD) pentru administratorul global sau pentru proprietarul grupului pentru a modifica grupul.</span><span class="sxs-lookup"><span data-stu-id="ce99f-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="ce99f-105">Înainte de a încerca să ștergeți un grup sincronizat din Azure AD, asigurați-vă că ați [șters toate licențele atribuite](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) pentru a evita erorile.</span><span class="sxs-lookup"><span data-stu-id="ce99f-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="ce99f-106">Pentru a înțelege cum să sincronizați utilizatori, grupuri și persoane de contact, consultați [AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)și urmați [sincronizarea unui grup local la AZURE folosind Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) pentru a sincroniza grupuri la-Perm folosind AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ce99f-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="ce99f-107">Urmați acest ghid pentru [Depanarea erorilor în timpul sincronizării](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) pentru a depana erorile comune în timpul sincronizării.</span><span class="sxs-lookup"><span data-stu-id="ce99f-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

