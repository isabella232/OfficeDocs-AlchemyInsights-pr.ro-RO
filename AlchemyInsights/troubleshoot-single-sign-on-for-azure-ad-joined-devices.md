---
title: Depanarea unui singur semn activat pentru dispozitivele Azure AD asociate
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037330"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="f43ed-102">Depanarea unui singur semn activat pentru dispozitivele Azure AD asociate</span><span class="sxs-lookup"><span data-stu-id="f43ed-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="f43ed-103">Dacă aveți un mediu Active Directory (AD) local și doriți să vă asociați la computerele asociate domeniului de publicitate la Azure AD, puteți realiza acest lucru efectuând asocierea hibrid Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f43ed-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="f43ed-104">Instrucțiuni [: planificarea implementării hibride Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vă oferă pașii asociați pentru a implementa un hibrid Azure AD Join în mediul dvs.</span><span class="sxs-lookup"><span data-stu-id="f43ed-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="f43ed-105">Pentru mai multe informații, consultați [Configurarea dispozitivelor asociate AZURE AD pentru Single-Sign local la utilizarea Windows Hello pentru Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="f43ed-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="f43ed-106">**Probleme principale de refresh token (PRT)**</span><span class="sxs-lookup"><span data-stu-id="f43ed-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="f43ed-107">Un simbol reîmprospătare principală (PRT) este un artefact cheie al autentificării Azure AD pe Windows 10, Windows Server 2016 și versiunile mai recente, iOS și dispozitivele Android.</span><span class="sxs-lookup"><span data-stu-id="f43ed-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="f43ed-108">Acesta este un token web JSON (JWT) emis special pentru brokerii de simboluri pentru prima parte din Microsoft pentru a activa sign-on unic (SSO) în aplicațiile utilizate pe acele dispozitive.</span><span class="sxs-lookup"><span data-stu-id="f43ed-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="f43ed-109">Pentru detalii despre modul în care este emis un PRT, utilizat și protejat pe dispozitivele Windows 10, consultați [ce este un token de reîmprospătare primară?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="f43ed-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="f43ed-110">**WamDefaultSet: Da și AzureADPrt: Da**</span><span class="sxs-lookup"><span data-stu-id="f43ed-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="f43ed-111">Aceste câmpuri indică dacă utilizatorul s-a autentificat cu succes la Azure AD la conectarea la dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="f43ed-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="f43ed-112">Dacă valorile **nu** sunt, se poate datora:</span><span class="sxs-lookup"><span data-stu-id="f43ed-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="f43ed-113">Cheie de stocare nepotrivită din TPM asociată dispozitivului la înregistrare (Verificați KeySignTest în timp ce lucrați cu ridicat)</span><span class="sxs-lookup"><span data-stu-id="f43ed-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="f43ed-114">ID de conectare alternativă</span><span class="sxs-lookup"><span data-stu-id="f43ed-114">Alternate Login ID</span></span>
- <span data-ttu-id="f43ed-115">Proxy HTTP negăsit</span><span class="sxs-lookup"><span data-stu-id="f43ed-115">HTTP Proxy not found</span></span>

<span data-ttu-id="f43ed-116">Pentru a depana dispozitivele utilizând comanda dsregcmd, consultați [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="f43ed-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
