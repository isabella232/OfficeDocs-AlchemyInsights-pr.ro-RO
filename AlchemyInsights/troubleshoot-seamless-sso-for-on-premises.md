---
title: Depanarea unui sign-on unic (SSO) fără sudură pentru local
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816352"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="c4737-102">Depanarea unui sign-on unic (SSO) fără sudură pentru local</span><span class="sxs-lookup"><span data-stu-id="c4737-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="c4737-103">Pentru a rezolva problemele cu sign-on unic (SSO) fără sudură, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="c4737-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="c4737-104">**Cum pot răsturna cheia de decriptare Kerberos a contului de computer AZUREADSSO?**</span><span class="sxs-lookup"><span data-stu-id="c4737-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="c4737-105">Vă recomandăm foarte mult să răsturnați cheia de decriptare Kerberos cel puțin la fiecare 30 de zile.</span><span class="sxs-lookup"><span data-stu-id="c4737-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="c4737-106">Pentru a face acest lucru manual, consultați [cum să răsturnați tastele Kerberos decriptare](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="c4737-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="c4737-107">**Configurarea SSO fără sudură**</span><span class="sxs-lookup"><span data-stu-id="c4737-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="c4737-108">Pentru a implementa SSO fără sudură, urmați pașii din [Azure Active Directory fără sudură sign-on unic: pornire rapidă](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="c4737-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="c4737-109">**Sfătuire**</span><span class="sxs-lookup"><span data-stu-id="c4737-109">**Advisory**</span></span>

- <span data-ttu-id="c4737-110">[Azure Active Directory fără sudură sign-on unic: întrebări frecvente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) -în acest articol, vom adresa întrebări frecvente despre Azure Active Directory fără sudură single Sign-On (SSO fără sudură).</span><span class="sxs-lookup"><span data-stu-id="c4737-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="c4737-111">Continuați să căutați conținut nou.</span><span class="sxs-lookup"><span data-stu-id="c4737-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="c4737-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) -acest articol oferă informații despre cum să efectuați solicitări de caracteristici sau să puneți întrebări tehnice despre SSO fără sudură.</span><span class="sxs-lookup"><span data-stu-id="c4737-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="c4737-113">**Depanarea**</span><span class="sxs-lookup"><span data-stu-id="c4737-113">**Troubleshoot**</span></span>

<span data-ttu-id="c4737-114">[Depanarea Azure Active Directory fără sudură sign-on unic](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) -acest articol vă ajută să găsiți informații despre depanarea problemelor comune cu privire la o singură Sign-On fără sudură Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c4737-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







