---
title: Probleme cu Mae
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250177"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="36b41-102">Probleme cu Mae</span><span class="sxs-lookup"><span data-stu-id="36b41-102">Issues with MFA</span></span>
<span data-ttu-id="36b41-103">Există câteva lucruri pentru a verifica dacă utilizatorii nu pot autentifica utilizând autentificarea multi-factor (MAE)</span><span class="sxs-lookup"><span data-stu-id="36b41-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="36b41-104">Utilizator afectate pot fi blocați în Azure Active Director Portal.</span><span class="sxs-lookup"><span data-stu-id="36b41-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="36b41-105">Dacă este cazul, autentificare încearcă pentru că anumit utilizator va fi negat automat.</span><span class="sxs-lookup"><span data-stu-id="36b41-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="36b41-106">Vă rugăm să urmaţi paşii din acest articol pentru a le debloca.</span><span class="sxs-lookup"><span data-stu-id="36b41-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="36b41-107">În cazul în care nu ajuta la deblocarea utilizatorul sau utilizatorul nu este blocat, puteţi încerca să resetaţi Mae pentru utilizator şi ei vor merge prin procesul de înscriere din nou.</span><span class="sxs-lookup"><span data-stu-id="36b41-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="36b41-108">Vă rugăm să urmaţi paşii din acest articol.</span><span class="sxs-lookup"><span data-stu-id="36b41-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="36b41-109">În cazul în care acest lucru este prima dată când aţi activat Mae şi utilizatorii sunt în imposibilitatea de a conecta la clientii non-browsere, cum ar fi Outlook, Skype, etc, poate ADAL (Active Director autentificare biblioteca) nu este activat pe abonamentul de O365.</span><span class="sxs-lookup"><span data-stu-id="36b41-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="36b41-110">În acest caz va trebui să conectaţi la Exchange Online Powershell şi de a executa acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="36b41-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>