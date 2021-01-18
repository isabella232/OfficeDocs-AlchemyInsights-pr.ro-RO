---
title: Configurarea proxy-ului aplicației
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885525"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="9ec17-102">Configurarea proxy-ului aplicației</span><span class="sxs-lookup"><span data-stu-id="9ec17-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="9ec17-103">Pentru a înțelege cum să configurați o aplicație proxy de aplicație din Azure AD pentru a expune aplicațiile locale în cloud, consultați [cum se configurează o aplicație proxy de aplicație](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="9ec17-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="9ec17-104">Sign-on unic (SSO) permite utilizatorilor să acceseze o aplicație fără a se autentifica de mai multe ori.</span><span class="sxs-lookup"><span data-stu-id="9ec17-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="9ec17-105">Permite autentificarea unică să aibă loc în cloud, împotriva Azure Active Directory și permite serviciului sau conectorului să imite utilizatorul pentru a finaliza toate provocările suplimentare de autentificare din aplicație.</span><span class="sxs-lookup"><span data-stu-id="9ec17-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="9ec17-106">Pentru a afla mai multe, consultați [cum se configurează sign-on unic la o aplicație proxy de aplicație](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="9ec17-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="9ec17-107">Utilizați [acest articol](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) pentru a depana problemele uzuale cu care se confruntă persoanele atunci când creați o aplicație proxy de aplicație nouă.</span><span class="sxs-lookup"><span data-stu-id="9ec17-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="9ec17-108">Dacă întâmpinați o problemă la configurarea autentificării back-end la aplicație, poate fi necesar să [depanați configurațiile de delegare constrânse Kerberos pentru proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) -ul aplicației sau să urmați instrucțiunile pentru [Configurarea aplicației cu PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) pentru a rezolva problema.</span><span class="sxs-lookup"><span data-stu-id="9ec17-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
