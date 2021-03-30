---
title: Probleme secrete ale clientului de înregistrare a aplicațiilor sau ale certificatelor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405335"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="e75c6-102">Probleme secrete ale clientului de înregistrare a aplicațiilor sau ale certificatelor</span><span class="sxs-lookup"><span data-stu-id="e75c6-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="e75c6-103">Clientul aplicației expiră secret?</span><span class="sxs-lookup"><span data-stu-id="e75c6-103">Application client secret expiring?</span></span>

<span data-ttu-id="e75c6-104">Indiferent cum a fost creată aplicația înregistrată, fie prin procesul de înregistrare standard din portalul de înregistrare a aplicațiilor, fie dacă entitatea principală de serviciu a fost creată în entitatea dvs. găzduită folosind consimțământul aplicației, va trebui creat un nou Secret client înainte de expirarea acestuia curent și actualizat în codul aplicației asociate.</span><span class="sxs-lookup"><span data-stu-id="e75c6-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="e75c6-105">Perioada maximă de validitate este de 2 ani.</span><span class="sxs-lookup"><span data-stu-id="e75c6-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="e75c6-106">Ca memento, valoarea secretă trebuie înregistrată, deoarece nu va mai fi vizibilă după ce părăsiți pagina de înregistrări a aplicațiilor din portal.</span><span class="sxs-lookup"><span data-stu-id="e75c6-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="e75c6-107">Pentru mai multe informații, consultați [Pornire rapidă: Înregistrați o](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplicație pe platforma de identitate Microsoft și Cele mai bune practici pentru platforma de identitate [Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="e75c6-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="e75c6-108">Pentru a afla mai multe, consultați Crearea unui cont principal de & de aplicație [Azure AD în portalul - platforma de identitate Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="e75c6-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
