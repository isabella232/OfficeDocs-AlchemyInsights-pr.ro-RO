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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768849"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="53115-102">Probleme cu Azure MFA</span><span class="sxs-lookup"><span data-stu-id="53115-102">Issues with Azure MFA</span></span>
<span data-ttu-id="53115-103">Există câteva lucruri pentru a verifica dacă utilizatorii nu pot conecta utilizând autentificarea multi-factor (MFA)</span><span class="sxs-lookup"><span data-stu-id="53115-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="53115-104">Utilizatorul afectat poate fi blocat în Azure Active Directory portal.</span><span class="sxs-lookup"><span data-stu-id="53115-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="53115-105">În acest caz, încercările de autentificare pentru acel utilizator specific vor fi refuzate automat.</span><span class="sxs-lookup"><span data-stu-id="53115-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="53115-106">Vă rugăm să urmați pașii din acest articol pentru a le debloca.</span><span class="sxs-lookup"><span data-stu-id="53115-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="53115-107">Dacă deblocarea utilizatorului nu a ajutat sau utilizatorul nu este blocat, puteți încerca să reinițializați MFA pentru utilizator și vor trece prin procesul de înscriere din nou.</span><span class="sxs-lookup"><span data-stu-id="53115-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="53115-108">Vă rugăm să urmați pașii din acest articol.</span><span class="sxs-lookup"><span data-stu-id="53115-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="53115-109">Dacă aceasta este prima dată când ați activat MFA și utilizatorii nu pot să se autentifice la clienții non-browsere, ar fi Outlook, Skype, etc, poate ADAL (Active Directory Authentication Library) nu este activată pe abonamentul O365.</span><span class="sxs-lookup"><span data-stu-id="53115-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="53115-110">În acest caz, va trebui să vă conectați la Exchange Online PowerShell și executați acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="53115-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>