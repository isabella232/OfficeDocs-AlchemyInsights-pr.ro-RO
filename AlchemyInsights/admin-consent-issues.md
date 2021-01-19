---
title: Probleme cu consimțământul administratorului
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901509"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="05d6b-102">Probleme cu consimțământul administratorului</span><span class="sxs-lookup"><span data-stu-id="05d6b-102">Admin consent issues</span></span>

1. <span data-ttu-id="05d6b-103">Activați [fluxul de lucru pentru consimțământul administratorului](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) pentru a permite utilizatorilor să solicite aprobarea de administrator direct din ecranul de consimțământ.</span><span class="sxs-lookup"><span data-stu-id="05d6b-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="05d6b-104">Dacă dumneavoastră sau utilizatorii aplicației Vedeți erori neașteptate în timpul procesului de consimțământ, consultați acest articol pentru pașii de depanare: [Eroare neașteptată atunci când efectuați consimțământul pentru o aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="05d6b-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="05d6b-105">Aflați mai multe despre [consimțământul administratorului pe platforma de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), modul în care funcționează [solicitarea de aprobare](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) și cum să [evaluați o solicitare pentru consimțământul administratorului la nivel de entitate găzduită](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="05d6b-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="05d6b-106">Aplicațiile care se integrează cu platforma de identitate Microsoft urmăresc un model de autorizare care le oferă utilizatorilor și administratorilor controlul asupra modului în care pot fi accesate datele.</span><span class="sxs-lookup"><span data-stu-id="05d6b-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="05d6b-107">Implementarea modelului de autorizare a fost actualizată pe punctul final al platformei de identitate Microsoft și schimbă modul în care o aplicație trebuie să interacționeze cu platforma de identitate Microsoft.</span><span class="sxs-lookup"><span data-stu-id="05d6b-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="05d6b-108">Vedeți [permisiunile și consimțământul în punctul final al platformei de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) pentru o prezentare generală a acestui model de autorizare, inclusiv domeniile, permisiunile și consimțământul.</span><span class="sxs-lookup"><span data-stu-id="05d6b-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>