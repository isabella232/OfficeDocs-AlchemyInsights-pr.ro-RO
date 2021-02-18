---
title: Gestionarea setărilor externe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294311"
---
# <a name="managing-external-settings"></a><span data-ttu-id="0f736-102">Gestionarea setărilor externe</span><span class="sxs-lookup"><span data-stu-id="0f736-102">Managing External Settings</span></span>

<span data-ttu-id="0f736-103">**Anunț**</span><span class="sxs-lookup"><span data-stu-id="0f736-103">**Announcement**</span></span>

- <span data-ttu-id="0f736-104">[Dezaprobarea suportului de conectare pentru vizualizare de la Google începând cu 4 ianuarie 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="0f736-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="0f736-105">Testați dacă aplicațiile sunt afectate, urmând instrucțiunile Google privind compatibilitatea testării</span><span class="sxs-lookup"><span data-stu-id="0f736-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="0f736-106">Asigurați-vă că utilizați vizualizarea web sistem sau browserul de sistem la conectarea utilizatorilor cu conturi Google pentru consumatori</span><span class="sxs-lookup"><span data-stu-id="0f736-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="0f736-107">**Gestionarea setărilor invitației**</span><span class="sxs-lookup"><span data-stu-id="0f736-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="0f736-108">Confirmați că ați [configurat setările de colaborare externă](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) pentru a permite persoanelor potrivite să trimită invitații.</span><span class="sxs-lookup"><span data-stu-id="0f736-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="0f736-109">**Gestionarea permisiunilor de acces ale utilizatorilor invitați**</span><span class="sxs-lookup"><span data-stu-id="0f736-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="0f736-110">Administratorii globali pot gestiona permisiunile de acces ale invitaților în director prin intermediul portalului Azure, configurând permisiunile de acces pentru invitați pe pagina Setări de colaborare externă.</span><span class="sxs-lookup"><span data-stu-id="0f736-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="0f736-111">[Aflați mai multe despre această setare](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0f736-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="0f736-112">Dacă doriți ca oaspeții dumneavoastră să acceseze aplicații, cum ar fi teams sau SharePoint, confirmați că ați configurat acele aplicații pentru a permite accesul invitaților.</span><span class="sxs-lookup"><span data-stu-id="0f736-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="0f736-113">Aflați mai multe despre [setările teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) și [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0f736-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0f736-114">**Configurarea invitațiilor:**</span><span class="sxs-lookup"><span data-stu-id="0f736-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="0f736-115">Activați colaborarea externă B2B și gestionarea persoanelor care pot invita invitați</span><span class="sxs-lookup"><span data-stu-id="0f736-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="0f736-116">Permiterea sau blocarea invitațiilor către utilizatori din anumite organizații</span><span class="sxs-lookup"><span data-stu-id="0f736-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="0f736-117">**Configurarea furnizorilor de identitate permiși:**</span><span class="sxs-lookup"><span data-stu-id="0f736-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="0f736-118">Federația Google</span><span class="sxs-lookup"><span data-stu-id="0f736-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="0f736-119">Federation direct</span><span class="sxs-lookup"><span data-stu-id="0f736-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="0f736-120">Autentificarea prin e-mail cu o singură dată</span><span class="sxs-lookup"><span data-stu-id="0f736-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
