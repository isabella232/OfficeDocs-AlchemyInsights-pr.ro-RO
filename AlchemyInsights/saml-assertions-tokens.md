---
title: Aserții SAML (tokenuri)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109252"
---
# <a name="saml-assertions-tokens"></a>Aserții SAML (tokenuri)

1. Simbolurile SAML (Security Assertions Markup Language) sunt reprezentări XML ale solicitărilor. În mod implicit, simbolurile SAML Windows Communication Foundation (WCF) în scenariile de securitate federativă sunt simboluri emise. Pentru mai multe informații, consultați [Tokenurile și solicitările SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. De Serviciu de identitate Microsoft emite mai multe tipuri de simboluri de securitate în procesarea fiecărui flux de autentificare. [Referința de solicitări de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descrie formatul, caracteristicile de securitate și conținutul simbolurilor SAML 2.0.
3. Urmați instrucțiunile din [Configurabil tokenul pe durata Serviciu de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) pentru a înțelege cum să configurați durata de viață a simbolurilor.
4. Urmați pașii subliniați în [acest articol pentru](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) a înțelege cum să configurați criptarea simbolurilor Azure AD SAML.
5. În Azure AD, puteți configura opțiunile de semnare a certificatelor și algoritmul de semnare a certificatelor. Pentru mai multe informații, consultați [Opțiuni complexe de semnare a certificatelor în simbolul SAML pentru aplicațiile de galerie Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
