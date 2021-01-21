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
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="112a1-102">Configurarea și extinderea duratei de viață a tokenului</span><span class="sxs-lookup"><span data-stu-id="112a1-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="112a1-103">Puteți specifica durata de viață a unui token Access, SAML sau ID emis de platforma de identitate Microsoft.</span><span class="sxs-lookup"><span data-stu-id="112a1-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="112a1-104">Puteți să setați vieți token pentru toate aplicațiile din organizație, pentru o aplicație cu mai multe entități găzduite (multi-organizație) sau pentru un anumit director de serviciu din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="112a1-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="112a1-105">Pentru mai multe informații, citiți [durata de viață a tokenurilor configurabile](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="112a1-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="112a1-106">Pentru exemple, citiți [exemple despre cum să configurați duratele de viață ale tokenului](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="112a1-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="112a1-107">Pentru a afla cum să configurați durata de viață și compatibilitatea unui simbol în Azure Active Directory B2C (Azure AD B2C), consultați [Configurarea tokenurilor în Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="112a1-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="112a1-108">Articolul [Configurarea comportamentului sesiunii în Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descrie metodele de sign-on unic (SSO) utilizate în AZURE AD B2C și vă ajută să alegeți metoda SSO cea mai potrivită atunci când configurați politica.</span><span class="sxs-lookup"><span data-stu-id="112a1-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="112a1-109">**Cât timp durează jetoanele? Cât timp sunt valabile?**</span><span class="sxs-lookup"><span data-stu-id="112a1-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="112a1-110">Durata de viață a tokenului este de 1 oră și durata sesiunii este de 24 de ore.</span><span class="sxs-lookup"><span data-stu-id="112a1-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="112a1-111">Acest lucru înseamnă că, dacă nu s-au efectuat solicitări în 24 de ore, va trebui să vă conectați din nou înainte de a solicita un nou token.</span><span class="sxs-lookup"><span data-stu-id="112a1-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="112a1-112">După 30 mai, 2020, nicio entitate găzduită nouă nu va putea să utilizeze Politica de durată a tokenului configurabil pentru a configura tichetele de sesiune și de reîmprospătare.</span><span class="sxs-lookup"><span data-stu-id="112a1-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="112a1-113">Dezaprobarea va avea loc în următoarele câteva luni, ceea ce înseamnă că nu vom mai onora sesiunea existentă și vom reîmprospăta poliția Tokens.</span><span class="sxs-lookup"><span data-stu-id="112a1-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="112a1-114">Puteți în continuare să configurați duratele de viață ale tokenului de acces după dezaprobare.</span><span class="sxs-lookup"><span data-stu-id="112a1-114">You can still configure access token lifetimes after the deprecation.</span></span>






