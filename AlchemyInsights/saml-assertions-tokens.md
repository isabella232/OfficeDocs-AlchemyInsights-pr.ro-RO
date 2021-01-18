---
title: Afirmații SAML (simboluri)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885673"
---
# <a name="saml-assertions-tokens"></a>Afirmații SAML (simboluri)

1. Simbolurile de securitate pentru afirmațiile de Markup Language (SAML) sunt reprezentări XML ale creanțelor. În mod implicit, utilizați token-ul Windows Communication Foundation (WCF) în scenariile de securitate federative. Pentru mai multe informații, consultați [SAML tokens și claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Platforma de identitate Microsoft emite mai multe tipuri de simboluri de securitate în procesarea fiecărui flux de autentificare. [Referința revendicărilor tokenului SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descrie formatul, caracteristicile de securitate și conținutul tokenurilor SAML 2,0.
3. Urmați instrucțiunile din [duratele de viață ale tokenurilor configurabile din platforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) pentru a înțelege cum să configurați viețile token.
4. Urmați pașii schițați în [acest articol](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) pentru a înțelege cum să configurați criptarea simbolurilor AZURE AD SAML.
5. În Azure AD, puteți să configurați opțiunile de semnare a certificatului și algoritmul de semnare a certificatului. Pentru mai multe informații, consultați [Opțiuni complexe de semnare a certificatelor din simbolul SAML pentru aplicațiile din galerie din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
