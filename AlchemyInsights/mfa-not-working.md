---
title: Probleme cu MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545189"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="002d0-102">Probleme cu MFA</span><span class="sxs-lookup"><span data-stu-id="002d0-102">Issues with MFA</span></span>
<span data-ttu-id="002d0-103">Există câteva lucruri pentru a verifica dacă utilizatorii nu pot login utilizând autentificarea multi-factor (MFA)</span><span class="sxs-lookup"><span data-stu-id="002d0-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="002d0-104">Utilizatorul afectat poate fi blocat în Azure Active Directory portal.</span><span class="sxs-lookup"><span data-stu-id="002d0-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="002d0-105">În acest caz, încercările de autentificare pentru acel utilizator specific vor fi refuzate automat.</span><span class="sxs-lookup"><span data-stu-id="002d0-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="002d0-106">Vă rugăm să urmați pașii din acest articol pentru a le debloca.</span><span class="sxs-lookup"><span data-stu-id="002d0-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="002d0-107">Dacă deblocarea utilizatorului nu a ajutat sau utilizatorul nu este blocat, puteți încerca să reinițializați MFA pentru utilizator și vor trece prin procesul de înscriere din nou.</span><span class="sxs-lookup"><span data-stu-id="002d0-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="002d0-108">Vă rugăm să urmați pașii din acest articol.</span><span class="sxs-lookup"><span data-stu-id="002d0-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="002d0-109">Dacă aceasta este prima dată când ați activat MFA și utilizatorii nu pot să se autentifice la clienții non-browsere, ar fi Outlook, Skype, etc, poate ADAL (Active Directory Authentication Library) nu este activată pe abonamentul O365.</span><span class="sxs-lookup"><span data-stu-id="002d0-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="002d0-110">În acest caz, va trebui să vă conectați la Exchange Online PowerShell și executați acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="002d0-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>