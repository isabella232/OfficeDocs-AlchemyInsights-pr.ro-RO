---
title: Configurarea și extinderea duratei de viață a tokenului
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917009"
---
# <a name="configure-and-extend-token-lifetimes"></a>Configurarea și extinderea duratei de viață a tokenului

Puteți specifica durata de viață a unui token Access, SAML sau ID emis de platforma de identitate Microsoft. Puteți să setați vieți token pentru toate aplicațiile din organizație, pentru o aplicație cu mai multe entități găzduite (multi-organizație) sau pentru un anumit director de serviciu din organizația dvs. Pentru mai multe informații, citiți [durata de viață a tokenurilor configurabile](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Pentru exemple, citiți [exemple despre cum să configurați duratele de viață ale tokenului](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Pentru a afla cum să configurați durata de viață și compatibilitatea unui simbol în Azure Active Directory B2C (Azure AD B2C), consultați [Configurarea tokenurilor în Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Articolul [Configurarea comportamentului sesiunii în Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descrie metodele de sign-on unic (SSO) utilizate în AZURE AD B2C și vă ajută să alegeți metoda SSO cea mai potrivită atunci când configurați politica.

**Cât timp durează jetoanele? Cât timp sunt valabile?**

Durata de viață a tokenului este de 1 oră și durata sesiunii este de 24 de ore. Acest lucru înseamnă că, dacă nu s-au efectuat solicitări în 24 de ore, va trebui să vă conectați din nou înainte de a solicita un nou token.

> [!NOTE]
> După 30 mai, 2020, nicio entitate găzduită nouă nu va putea să utilizeze Politica de durată a tokenului configurabil pentru a configura tichetele de sesiune și de reîmprospătare. Dezaprobarea va avea loc în următoarele câteva luni, ceea ce înseamnă că nu vom mai onora sesiunea existentă și vom reîmprospăta poliția Tokens. Puteți în continuare să configurați duratele de viață ale tokenului de acces după dezaprobare.






