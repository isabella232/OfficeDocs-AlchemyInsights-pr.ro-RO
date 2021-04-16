---
title: Probleme cu MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810496"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="8ca2d-102">Probleme cu Azure MFA</span><span class="sxs-lookup"><span data-stu-id="8ca2d-102">Issues with Azure MFA</span></span>
<span data-ttu-id="8ca2d-103">Există câteva lucruri de verificat dacă utilizatorii nu se pot conecta utilizând Multi-Factor Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="8ca2d-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="8ca2d-104">Este posibil ca utilizatorul afectat să fie blocat în portalul Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8ca2d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="8ca2d-105">În acest caz, încercările de autentificare pentru acel utilizator vor fi refuzate automat.</span><span class="sxs-lookup"><span data-stu-id="8ca2d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="8ca2d-106">Urmați pașii din acest articol pentru a le debloca.</span><span class="sxs-lookup"><span data-stu-id="8ca2d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="8ca2d-107">Dacă deblocarea utilizatorului nu a fost de ajutor sau dacă utilizatorul nu este blocat, puteți încerca să resetați MFA pentru utilizator și acesta va trece din nou prin procesul de înscriere.</span><span class="sxs-lookup"><span data-stu-id="8ca2d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="8ca2d-108">Urmați pașii din acest articol.</span><span class="sxs-lookup"><span data-stu-id="8ca2d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="8ca2d-109">Dacă aceasta este prima dată când activați MFA și utilizatorii dvs. nu se pot conecta la clienți non-browser, cum ar fi Outlook, Skype etc, poate că ADAL (Active Directory Authentication Library) nu este activat în abonamentul dvs. O365.</span><span class="sxs-lookup"><span data-stu-id="8ca2d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="8ca2d-110">În acest caz, va trebui să vă conectați la Exchange Online Powershell și să rulați acest cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="8ca2d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>