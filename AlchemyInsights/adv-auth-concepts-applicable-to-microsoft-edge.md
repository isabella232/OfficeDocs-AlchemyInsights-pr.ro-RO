---
title: Concepte de autentificare avansate care se aplică Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934377"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concepte de autentificare avansate care se aplică Microsoft Edge

În cele ce urmează urmează conceptele de autentificare avansate care se aplică Microsoft Edge:

**Autentificare proactivă**

Atunci când activați [politica ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge va încerca să autentifice proactiv utilizatorii autentificați prin servicii Microsoft. La intervale regulate, acesta va utiliza un serviciu online pentru a căuta un manifest actualizat care conține configurația care guvernează autentificarea Proactivă.

Avantaje: Autentificarea proactivă permite autentificarea la servicii cheie, cum ar fi pagina Office filă nouă. De asemenea, Bing este utilizată ca motor de căutare, Autentificarea proactivă îmbunătățește performanța barei de adrese și vă ajută să generați rezultate de căutare personalizate pentru necesitățile afacerii dvs.

**Windows Hello CredUI pentru autentificare NTLM**

Dacă caracteristica sign-on unic (SSO) nu este disponibilă atunci când un site web încearcă să se conecteze la utilizator prin mecanismul NTLM sau Negociați, această caracteristică va permite utilizatorului să partajeze acreditările OS cu site-ul web și să îndeplinească provocarea autentificării utilizând interfața utilizator Windows Hello Cred. Acest flux de sign-on va apărea doar în Windows 10 și doar pentru utilizatorii care nu primesc SSO în timpul unei NTLM sau a unei provocări de negociare.

**Utilizați parole salvate pentru a vă conecta automat**

Utilizatorii care salvează parole în Microsoft Edge pot activa conectarea automată la site-urile web unde au salvat acreditări. Utilizatorii pot activa sau dezactiva această caracteristică edge://settings/passwords și o puteți configura în politicile [managerului](https://go.microsoft.com/fwlink/?linkid=2134622) de parole.
