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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="757bd-102">Afirmații SAML (simboluri)</span><span class="sxs-lookup"><span data-stu-id="757bd-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="757bd-103">Simbolurile de securitate pentru afirmațiile de Markup Language (SAML) sunt reprezentări XML ale creanțelor.</span><span class="sxs-lookup"><span data-stu-id="757bd-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="757bd-104">În mod implicit, utilizați token-ul Windows Communication Foundation (WCF) în scenariile de securitate federative.</span><span class="sxs-lookup"><span data-stu-id="757bd-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="757bd-105">Pentru mai multe informații, consultați [SAML tokens și claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="757bd-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="757bd-106">Platforma de identitate Microsoft emite mai multe tipuri de simboluri de securitate în procesarea fiecărui flux de autentificare.</span><span class="sxs-lookup"><span data-stu-id="757bd-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="757bd-107">[Referința revendicărilor tokenului SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descrie formatul, caracteristicile de securitate și conținutul tokenurilor SAML 2,0.</span><span class="sxs-lookup"><span data-stu-id="757bd-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="757bd-108">Urmați instrucțiunile din [duratele de viață ale tokenurilor configurabile din platforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) pentru a înțelege cum să configurați viețile token.</span><span class="sxs-lookup"><span data-stu-id="757bd-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="757bd-109">Urmați pașii schițați în [acest articol](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) pentru a înțelege cum să configurați criptarea simbolurilor AZURE AD SAML.</span><span class="sxs-lookup"><span data-stu-id="757bd-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="757bd-110">În Azure AD, puteți să configurați opțiunile de semnare a certificatului și algoritmul de semnare a certificatului.</span><span class="sxs-lookup"><span data-stu-id="757bd-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="757bd-111">Pentru mai multe informații, consultați [Opțiuni complexe de semnare a certificatelor din simbolul SAML pentru aplicațiile din galerie din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="757bd-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
