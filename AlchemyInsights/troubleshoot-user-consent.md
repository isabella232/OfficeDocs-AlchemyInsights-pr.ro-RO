---
title: Depanarea consimțământului utilizatorului
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901632"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="dd24b-102">Depanarea consimțământului utilizatorului</span><span class="sxs-lookup"><span data-stu-id="dd24b-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="dd24b-103">Puteți configura modul în care utilizatorii finali sunt consimțământul aplicațiilor prin portalul Azure sau PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dd24b-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="dd24b-104">Consultați [setările de consimțământ pentru utilizatori](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="dd24b-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="dd24b-105">De asemenea, un administrator poate utiliza [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) pentru a acorda consimțământul permisiunilor delegate în numele unui singur utilizator.</span><span class="sxs-lookup"><span data-stu-id="dd24b-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="dd24b-106">Pentru mai multe informații, consultați [Obțineți acces în numele unui utilizator](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="dd24b-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="dd24b-107">[Erorile de consimțământ pentru utilizator](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): acest articol discută despre erorile care pot apărea în timpul procesului de consimțire la o aplicație.</span><span class="sxs-lookup"><span data-stu-id="dd24b-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="dd24b-108">Dacă depanați solicitările de consimțământ neașteptate care nu conțin mesaje de eroare, consultați [scenarii de autentificare pentru AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="dd24b-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>