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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545189"
---
# <a name="issues-with-mfa"></a>Probleme cu Mae
Există câteva lucruri pentru a verifica dacă utilizatorii nu pot autentifica utilizând autentificarea multi-factor (MAE)

1. Utilizator afectate pot fi blocați în Azure Active Director Portal. Dacă este cazul, autentificare încearcă pentru că anumit utilizator va fi negat automat. [Vă rugăm să urmaţi paşii din acest articol pentru a le debloca.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. În cazul în care nu ajuta la deblocarea utilizatorul sau utilizatorul nu este blocat, puteţi încerca să resetaţi Mae pentru utilizator şi ei vor merge prin procesul de înscriere din nou. [Vă rugăm să urmaţi paşii din acest articol.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

În cazul în care acest lucru este prima dată când aţi activat Mae şi utilizatorii sunt în imposibilitatea de a conecta la clientii non-browsere, cum ar fi Outlook, Skype, etc, poate ADAL (Active Director autentificare biblioteca) nu este activat pe abonamentul de O365. În acest caz va trebui să conectaţi la Exchange Online Powershell şi de a executa acest cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*