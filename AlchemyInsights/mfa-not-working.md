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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098614"
---
# <a name="issues-with-azure-mfa"></a>Probleme cu Azure MFA
Există câteva lucruri de verificat dacă utilizatorii nu se pot conecta utilizând Multi-Factor Authentication (MFA)

1. Este posibil ca utilizatorul afectat să fie blocat Azure Active Directory Portal. În acest caz, încercările de autentificare pentru acel utilizator vor fi refuzate automat. [Urmați pașii din acest articol pentru a le debloca.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Dacă deblocarea utilizatorului nu a fost de ajutor sau dacă utilizatorul nu este blocat, puteți încerca să resetați MFA pentru utilizator și acesta va trece din nou prin procesul de înscriere. [Urmați pașii din acest articol.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Dacă aceasta este prima dată când activați MFA și utilizatorii dvs. nu se pot conecta la clienți non-browser, cum ar fi Outlook, Skype etc, poate că ADAL (Active Directory Authentication Library) nu este activat în abonamentul dvs. O365. În acest caz, va trebui să vă conectați la Exchange Online Powershell și să rulați acest cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*