---
title: Problemă de asigurare a accesului SCIM
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949945"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="e92ae-102">Problemă de asigurare a accesului SCIM</span><span class="sxs-lookup"><span data-stu-id="e92ae-102">SCIM provisioning issue</span></span>

<span data-ttu-id="e92ae-103">Asigurarea accesului automat se referă la crearea de identități de utilizator și roluri în aplicațiile Cloud la care au nevoie utilizatorii.</span><span class="sxs-lookup"><span data-stu-id="e92ae-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="e92ae-104">În plus față de crearea de identități de utilizator, asigurarea accesului automat include întreținerea și eliminarea identităților de utilizator ca modificări ale stării sau rolurilor.</span><span class="sxs-lookup"><span data-stu-id="e92ae-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="e92ae-105">Înainte de a începe o implementare, puteți revizui [modul](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) în care funcționează asigurarea accesului pentru a afla cum funcționează dispoziția Azure Active Directory (AD) și pentru a obține recomandări de configurare.</span><span class="sxs-lookup"><span data-stu-id="e92ae-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="e92ae-106">Ca dezvoltator de aplicații, puteți să utilizați API-ul de gestionare a utilizatorilor pentru gestionarea identității prin domenii (SCIM) pentru a activa asigurarea accesului automat al utilizatorilor și grupurilor între aplicație și Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e92ae-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="e92ae-107">[Compilarea unui punct final SCIM și configurarea accesului utilizatorilor cu un articol AZURE AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) descrie cum să creați un punct final SCIM și să-l integrați cu serviciul de asigurare a accesului la Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e92ae-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



