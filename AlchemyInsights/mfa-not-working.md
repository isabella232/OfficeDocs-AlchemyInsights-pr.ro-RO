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
# <a name="issues-with-mfa"></a>Probleme cu Mae
Există câteva lucruri pentru a verifica dacă utilizatorii nu pot autentifica utilizând autentificarea multi-factor (MAE)

1. Utilizator afectate pot fi blocați în Azure Active Director Portal. Dacă este cazul, autentificare încearcă pentru că anumit utilizator va fi negat automat. [Vă rugăm să urmaţi paşii din acest articol pentru a le debloca.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. În cazul în care nu ajuta la deblocarea utilizatorul sau utilizatorul nu este blocat, puteţi încerca să resetaţi Mae pentru utilizator şi ei vor merge prin procesul de înscriere din nou. [Vă rugăm să urmaţi paşii din acest articol.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

În cazul în care acest lucru este prima dată când aţi activat Mae şi utilizatorii sunt în imposibilitatea de a conecta la clientii non-browsere, cum ar fi Outlook, Skype, etc, poate ADAL (Active Director autentificare biblioteca) nu este activat pe abonamentul de O365. În acest caz va trebui să conectaţi la Exchange Online Powershell şi de a executa acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*