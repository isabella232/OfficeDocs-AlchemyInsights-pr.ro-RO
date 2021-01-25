---
title: Permisiuni și consimțământ pentru API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974991"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="327f0-102">Permisiuni și consimțământ pentru API</span><span class="sxs-lookup"><span data-stu-id="327f0-102">API permissions and consent</span></span>

<span data-ttu-id="327f0-103">Aplicațiile care se integrează cu platforma de identitate Microsoft urmăresc un model de autorizare care le oferă utilizatorilor și administratorilor controlul asupra modului în care pot fi accesate datele.</span><span class="sxs-lookup"><span data-stu-id="327f0-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="327f0-104">Implementarea modelului de autorizare a fost actualizată pe punctul final al platformei de identitate Microsoft.</span><span class="sxs-lookup"><span data-stu-id="327f0-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="327f0-105">Acesta modifică modul în care o aplicație trebuie să interacționeze cu platforma de identitate Microsoft.</span><span class="sxs-lookup"><span data-stu-id="327f0-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="327f0-106">[Permisiunile și consimțământul în punctul final al platformei de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) acoperă conceptele de bază ale acestui model de autorizare, inclusiv domeniile, permisiunile și consimțământul.</span><span class="sxs-lookup"><span data-stu-id="327f0-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="327f0-107">Framework-ul de [consimțământ Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) vă ajută să dezvoltați mai ușor aplicații client web și nativi cu mai mulți entități găzduite.</span><span class="sxs-lookup"><span data-stu-id="327f0-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="327f0-108">Aceste aplicații permit conectarea de către conturile de utilizator de la o entitate găzduită Azure AD care diferă de cea în care este înregistrată aplicația.</span><span class="sxs-lookup"><span data-stu-id="327f0-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="327f0-109">De asemenea, poate fi necesar să acceseze API-uri web, cum ar fi Microsoft Graph API (pentru a accesa Azure AD, Intune și Services în Microsoft 365) și alte API-uri de servicii Microsoft, în plus față de propriile API-uri web.</span><span class="sxs-lookup"><span data-stu-id="327f0-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

