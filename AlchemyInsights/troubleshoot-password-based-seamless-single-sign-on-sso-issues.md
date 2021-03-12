---
title: Depanarea problemelor cu sign-on unic (SSO) bazate pe parole
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714884"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="9ab51-102">Depanarea problemelor cu sign-on unic (SSO) bazate pe parole</span><span class="sxs-lookup"><span data-stu-id="9ab51-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="9ab51-103">Pentru a afla fundamentele SSO bazat pe parole, consultați [autentificarea bazată pe parolă cu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="9ab51-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="9ab51-104">**Configurarea SSO bazat pe parole**</span><span class="sxs-lookup"><span data-stu-id="9ab51-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="9ab51-105">[Configurați sign-on unic bazat pe parolă](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -acest articol intră în mai multe detalii despre opțiunea SSO bazat pe parolă.</span><span class="sxs-lookup"><span data-stu-id="9ab51-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="9ab51-106">Dacă aplicația pe care o adăugați necesită configurare particularizată și trebuie să utilizați SSO bazat pe parole, acest articol este pentru dvs.</span><span class="sxs-lookup"><span data-stu-id="9ab51-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="9ab51-107">[Configurarea unui singur semn bazat pe parolă pentru aplicațiile on-Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -proxy-ul aplicației acceptă mai multe moduri de sign-on unic.</span><span class="sxs-lookup"><span data-stu-id="9ab51-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="9ab51-108">Sign-on bazat pe parolă este destinat aplicațiilor care utilizează o combinație de nume de utilizator/parolă pentru autentificare.</span><span class="sxs-lookup"><span data-stu-id="9ab51-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="9ab51-109">Atunci când configurați sign-on bazat pe parolă pentru aplicație, utilizatorii trebuie să se conecteze o dată la aplicația locală.</span><span class="sxs-lookup"><span data-stu-id="9ab51-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="9ab51-110">După aceea, Azure Active Directory stochează informațiile de conectare și le furnizează automat aplicației atunci când utilizatorii îl accesează de la distanță.</span><span class="sxs-lookup"><span data-stu-id="9ab51-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="9ab51-111">Ar fi trebuit să aveți deja publicat și testat aplicația cu proxy de aplicație.</span><span class="sxs-lookup"><span data-stu-id="9ab51-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="9ab51-112">Dacă nu, urmați pașii din [publicarea aplicațiilor folosind proxy-ul aplicației AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , apoi continuați configurația SSO bazat pe parole pentru aplicațiile on-Prem.</span><span class="sxs-lookup"><span data-stu-id="9ab51-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="9ab51-113">Pentru a depana SSO bazat pe parole, consultați [Depanarea conectării unice bazate pe parolă în AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="9ab51-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
