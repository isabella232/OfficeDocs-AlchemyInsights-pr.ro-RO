---
title: Rezolvarea problemelor de autentificare SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826427"
---
# <a name="solving-smtp-authentication-issues"></a>Rezolvarea problemelor de autentificare SMTP

Dacă primiți erorile 5.7.57 sau 5.7.3 atunci când căutați să trimiteți mesaje de e-mail SMTP și să vă autentificați cu un client sau cu o aplicație, există câteva lucruri pe care ar trebui să le verificați:

- Remiterea SMTP autentificată poate fi dezactivată în entitatea dvs. găzduită sau în cutia poștală pe care încearcă să o utilizați (verificați ambele setări). Pentru a citi mai multe, consultați [Activarea sau dezactivarea remiterii SMTP client autentificat.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Verificați dacă [sunt activate valorile implicite de](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) securitate Azure pentru entitatea dvs. găzduită; Dacă este activată, autentificarea SMTP utilizând autentificarea de bază (numită și moștenit; aceasta va utiliza numele de utilizator și parola) nu va reuși.
