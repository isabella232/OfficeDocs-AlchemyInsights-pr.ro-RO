---
title: Maparea atributului de asigurare a accesului utilizatorilor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949893"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="264d3-102">Maparea atributului de asigurare a accesului utilizatorilor</span><span class="sxs-lookup"><span data-stu-id="264d3-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="264d3-103">Pentru a depana problemele cunoscute de mapare a atributelor, consultați [asocierile atributurilor](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="264d3-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="264d3-104">Microsoft Azure Active Directory (AD) oferă suport pentru asigurarea accesului utilizatorilor la aplicații SaaS de la terți, cum ar fi Salesforce, G Suite și altele.</span><span class="sxs-lookup"><span data-stu-id="264d3-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="264d3-105">Dacă activați asigurarea accesului utilizatorilor pentru o aplicație SaaS de la terți, portalul Azure controlează valorile sale de atribut prin mapări de atribute.</span><span class="sxs-lookup"><span data-stu-id="264d3-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="264d3-106">Pentru a afla cum să particularizați mapările de atribute implicite, consultați [Particularizarea atributului de asigurare a accesului utilizatorilor-mapări pentru aplicațiile SaaS din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="264d3-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="264d3-107">Pentru a afla mai multe despre asigurarea accesului utilizatorilor de aplicații SaaS, consultați [ce este asigurarea accesului utilizatorilor automat SaaS App în AZURE AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="264d3-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="264d3-108">Atunci când particularizați mapări de atribute pentru asigurarea accesului utilizatorilor, este posibil să descoperiți că atributul pe care doriți să îl mapați nu apare în lista de atribute sursă.</span><span class="sxs-lookup"><span data-stu-id="264d3-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="264d3-109">[Sincronizarea unui atribut din Active Directory local la AZURE AD pentru asigurarea accesului la un](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) articol de aplicație vă arată cum să adăugați atributul lipsă, dacă îl sincronizați de la reclama locală la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="264d3-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
