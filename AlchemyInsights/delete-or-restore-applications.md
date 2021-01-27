---
title: Ștergerea sau restaurarea aplicațiilor
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014908"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="8d222-102">Ștergerea sau restaurarea aplicațiilor</span><span class="sxs-lookup"><span data-stu-id="8d222-102">Delete or restore applications</span></span>

<span data-ttu-id="8d222-103">**Pentru a șterge o aplicație din entitatea găzduită AZURE AD**:</span><span class="sxs-lookup"><span data-stu-id="8d222-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="8d222-104">În **portalul AZURE AD**, selectați **aplicații de întreprindere**.</span><span class="sxs-lookup"><span data-stu-id="8d222-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="8d222-105">Apoi găsiți și selectați aplicația pe care doriți să o ștergeți.</span><span class="sxs-lookup"><span data-stu-id="8d222-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="8d222-106">În secțiunea **gestionare** din panoul din stânga, selectați **Proprietăți**.</span><span class="sxs-lookup"><span data-stu-id="8d222-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="8d222-107">Selectați **Ștergere**, apoi selectați **Da** pentru a confirma că doriți să ștergeți aplicația de la entitatea găzduită Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d222-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="8d222-108">Pentru mai multe informații despre cum să ștergeți o aplicație, consultați [pornire rapidă: ștergerea unei aplicații din entitatea găzduită Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="8d222-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="8d222-109">În PowerShell, cmdletul [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) elimină configurațiile proxy ale aplicației dintr-o anumită aplicație din Azure Active Directory și poate șterge complet aplicația dacă este specificată.</span><span class="sxs-lookup"><span data-stu-id="8d222-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="8d222-110">Puteți **restaura o aplicație ștearsă** utilizând PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8d222-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="8d222-111">După ce aplicația pe care doriți să o restaurați a fost identificată, puteți să o restaurați utilizând [Restaurare-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="8d222-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
