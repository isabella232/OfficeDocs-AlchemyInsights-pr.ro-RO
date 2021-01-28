---
title: Probleme cu revendicările și atributele token
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035970"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="8ffb6-102">Probleme cu revendicările și atributele token</span><span class="sxs-lookup"><span data-stu-id="8ffb6-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="8ffb6-103">**Actualizarea, configurarea sau eliminarea revendicărilor token**</span><span class="sxs-lookup"><span data-stu-id="8ffb6-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="8ffb6-104">Utilizând Azure Active Directory (Azure AD), puteți [particulariza tipul de revendicare pentru revendicarea rolului](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) în simbolul de răspuns pe care îl primiți după ce autorizați o aplicație.</span><span class="sxs-lookup"><span data-stu-id="8ffb6-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="8ffb6-105">Dezvoltatorii de aplicații pot utiliza revendicări opționale în aplicațiile lor Azure AD pentru a specifica ce revendicări doresc în tokenuri trimise aplicației.</span><span class="sxs-lookup"><span data-stu-id="8ffb6-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="8ffb6-106">Pentru mai multe informații, consultați [furnizarea de solicitări opționale la aplicație](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="8ffb6-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="8ffb6-107">[Configurați revendicările de grup pentru aplicațiile cu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="8ffb6-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="8ffb6-108">Dacă utilizați sign-on unic fără sudură în aplicația dvs., consultați [Particularizarea creanțelor emise în fișierul SAML pentru aplicațiile Enterprise](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="8ffb6-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="8ffb6-109">**Maparea atributului revendicări**</span><span class="sxs-lookup"><span data-stu-id="8ffb6-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="8ffb6-110">Pentru a configura politica de mapare a revendicărilor utilizând PowerShell, consultați [Particularizarea creanțelor emise în tokenuri pentru o anumită aplicație într-o entitate găzduită (Previzualizare)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="8ffb6-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="8ffb6-111">Atributele de extensie a schemelor directoare oferă o modalitate de a stoca date suplimentare în Azure Active Directory pentru obiectele de utilizator și alte obiecte din Director, cum ar fi grupuri, detalii despre entități găzduite, directori de servicii.</span><span class="sxs-lookup"><span data-stu-id="8ffb6-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="8ffb6-112">Numai atributele de extensie pentru obiectele de utilizator pot fi utilizate pentru emiterea de revendicări la aplicații.</span><span class="sxs-lookup"><span data-stu-id="8ffb6-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="8ffb6-113">[Utilizarea atributelor de extensie a schemelor directoare din revendicări](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) descrie modul în care se utilizează atributele de extensie a schemelor directoare pentru trimiterea datelor de utilizator la aplicațiile din revendicările token.</span><span class="sxs-lookup"><span data-stu-id="8ffb6-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="8ffb6-114">Pentru mai multe informații despre revendicările Token, consultați:</span><span class="sxs-lookup"><span data-stu-id="8ffb6-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="8ffb6-115">Revendicări în jetoanele Access</span><span class="sxs-lookup"><span data-stu-id="8ffb6-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="8ffb6-116">Creanțe într-o id_token</span><span class="sxs-lookup"><span data-stu-id="8ffb6-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="8ffb6-117">[Afirmațiile](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) la care vă puteți aștepta în tokenuri ID și simboluri de acces emise de AZURE AD B2C</span><span class="sxs-lookup"><span data-stu-id="8ffb6-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="8ffb6-118">Referință pentru revendicările tokenului SAML</span><span class="sxs-lookup"><span data-stu-id="8ffb6-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
