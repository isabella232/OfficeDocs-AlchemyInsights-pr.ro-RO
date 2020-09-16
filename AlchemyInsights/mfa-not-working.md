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
# <a name="issues-with-azure-mfa"></a>Probleme cu Azure Mae
Există câteva lucruri de verificat dacă utilizatorii nu se pot conecta utilizând autentificarea multi-factor (AMF)

1. Utilizatorul afectat poate fi blocat în portalul Azure Active Directory. Dacă acesta este cazul, încercările de autentificare pentru acel utilizator specific vor fi refuzate automat. [Vă rugăm să urmați pașii din acest articol pentru a-i debloca.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Dacă deblocarea utilizatorului nu a ajutat sau utilizatorul nu este blocat, puteți încerca să resetați Mae pentru utilizator și va trece din nou prin procesul de înscriere. [Vă rugăm să urmați pașii din acest articol.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Dacă aceasta este prima dată când ați activat Mae și utilizatorii nu se pot conecta la clienții care nu sunt browsere, cum ar fi Outlook, Skype etc., poate Monica (Active Directory Authentication Library) nu este activat în abonamentul O365. În acest caz, va trebui să vă conectați la Exchange Online PowerShell și să difuzați acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*