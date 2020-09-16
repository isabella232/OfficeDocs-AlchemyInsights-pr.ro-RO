---
title: Probleme cu Mae
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755143"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="7ecdd-102">Probleme cu Azure Mae</span><span class="sxs-lookup"><span data-stu-id="7ecdd-102">Issues with Azure MFA</span></span>
<span data-ttu-id="7ecdd-103">Există câteva lucruri de verificat dacă utilizatorii nu se pot conecta utilizând autentificarea multi-factor (AMF)</span><span class="sxs-lookup"><span data-stu-id="7ecdd-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="7ecdd-104">Utilizatorul afectat poate fi blocat în portalul Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7ecdd-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="7ecdd-105">Dacă acesta este cazul, încercările de autentificare pentru acel utilizator specific vor fi refuzate automat.</span><span class="sxs-lookup"><span data-stu-id="7ecdd-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="7ecdd-106">Vă rugăm să urmați pașii din acest articol pentru a-i debloca.</span><span class="sxs-lookup"><span data-stu-id="7ecdd-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="7ecdd-107">Dacă deblocarea utilizatorului nu a ajutat sau utilizatorul nu este blocat, puteți încerca să resetați Mae pentru utilizator și va trece din nou prin procesul de înscriere.</span><span class="sxs-lookup"><span data-stu-id="7ecdd-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="7ecdd-108">Vă rugăm să urmați pașii din acest articol.</span><span class="sxs-lookup"><span data-stu-id="7ecdd-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="7ecdd-109">Dacă aceasta este prima dată când ați activat Mae și utilizatorii nu se pot conecta la clienții care nu sunt browsere, cum ar fi Outlook, Skype etc., poate Monica (Active Directory Authentication Library) nu este activat în abonamentul O365.</span><span class="sxs-lookup"><span data-stu-id="7ecdd-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="7ecdd-110">În acest caz, va trebui să vă conectați la Exchange Online PowerShell și să difuzați acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="7ecdd-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>