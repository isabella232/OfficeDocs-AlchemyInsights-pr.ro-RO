---
title: Concepte de autentificare avansate care se aplică la Microsoft Edge
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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398597"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Concepte de autentificare avansate care se aplică la Microsoft Edge

În cele ce urmează conceptele de autentificare avansate care se aplică la Microsoft Edge:

**Autentificare proactivă**

Atunci când activați [politica ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge va încerca să autentifice proactiv utilizatorii autentificați prin intermediul serviciilor Microsoft. La intervale regulate, acesta va utiliza un serviciu online pentru a căuta un manifest actualizat care conține configurația care guvernează autentificarea Proactivă.

Avantaje: Autentificarea proactivă permite autentificarea la servicii cheie, cum ar fi pagina Filă nouă Office. De asemenea, dacă Bing este utilizat ca motor de căutare, Autentificarea proactivă îmbunătățește performanța barei de adrese și vă ajută să generați rezultate de căutare personalizate pentru necesitățile firmei dvs.

**Windows Hello CredUI pentru autentificare NTLM**

Dacă caracteristica sign-on unic (SSO) nu este disponibilă atunci când un site web încearcă să se conecteze la utilizator prin intermediul mecanismului NTLM sau Negociați, această caracteristică va permite utilizatorului să partajeze acreditările sistemului de operare cu site-ul web și să îndeplinească provocarea autentificării utilizând interfața utilizator Windows Hello Cred. Acest flux de sign-on va apărea doar în Windows 10 și doar pentru utilizatorii care nu primesc SSO în timpul unei proceduri NTLM sau a unei provocări de negociare.

**Utilizați parole salvate pentru a vă conecta automat**

Utilizatorii care salvează parole în Microsoft Edge pot activa conectarea automată la site-urile web unde au salvat acreditări. Utilizatorii pot activa sau dezactiva această caracteristică edge://settings/passwords și o puteți configura în politicile [managerului](https://go.microsoft.com/fwlink/?linkid=2134622) de parole.
