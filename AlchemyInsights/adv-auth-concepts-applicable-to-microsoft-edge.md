---
title: Concepte de autentificare complexe aplicabile în Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573528"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concepte de autentificare complexe aplicabile în Microsoft Edge

În continuare se află conceptele de autentificare avansată care se aplică la Microsoft Edge:

**Autentificarea proactivă**

Atunci când activați politica [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge va încerca să autentifice proactiv utilizatori conectați prin intermediul serviciilor Microsoft. La intervale regulate, acesta va utiliza un serviciu online pentru a căuta un manifest actualizat care conține configurația care reglementează autentificarea proactivă.

Beneficii: autentificarea proactivă permite autentificarea la servicii cheie, cum ar fi pagina filă nouă Office. De asemenea, dacă Bing este utilizat ca motor de căutare, autentificarea proactivă îmbunătățește performanța barei de adrese și ajută la generarea rezultatelor de căutare personalizate nevoilor firmei dvs.

**Windows Hello CredUI pentru autentificarea NTLM**

Dacă sign-on unic (SSO) nu este disponibil atunci când un site Web încearcă să se conecteze la utilizator prin mecanismul NTLM sau negociere, această caracteristică îi va permite utilizatorului să partajeze acreditările de sistem de operare cu site-ul web și să satisfacă provocarea de autentificare utilizând Windows Hello cred UI. Acest flux de sign-on va apărea doar în Windows 10 și doar pentru utilizatorii care nu obțin SSO în timpul unei contestații NTLM sau negociere.

**Utilizarea parolelor salvate pentru a vă conecta automat**

Utilizatorii care salvează parole în Microsoft Edge pot activa conectarea automată la site-uri web în care au salvat acreditările. Utilizatorii pot activa sau dezactiva această caracteristică în edge://settings/passwords și o puteți configura în politicile [Manager parole](https://go.microsoft.com/fwlink/?linkid=2134622) .
