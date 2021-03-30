---
title: Single-Sign activat pentru dispozitivele la care s-a alăturat Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405658"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="6d990-102">Sign-on unic pentru dispozitivele la care s-a alăturat Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6d990-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="6d990-103">Dacă aveți un mediu Local Active Directory (AD) și doriți să vă asociați computerelor care au domeniul unit cu Azure AD, puteți realiza acest lucru prin asocierea hibridă Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6d990-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="6d990-104">[Modul către: Planificarea implementării](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) hibride de asociere la Azure Active Directory vă furnizează pașii asociați pentru a implementa o asociere Azure AD hibridă în mediul dvs.</span><span class="sxs-lookup"><span data-stu-id="6d990-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="6d990-105">Configurarea dispozitivelor cu asociere Azure AD pentru dispozitive Single-Sign local utilizând Windows Hello pentru business</span><span class="sxs-lookup"><span data-stu-id="6d990-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="6d990-106">**Probleme principale cu tokenul de reîmprospătare (PRT)** Un token de reîmprospătare principal (PRT) este un artefact cheie de autentificare Azure AD pe dispozitive Windows 10, Windows Server 2016 și versiuni mai recente, iOS și Android.</span><span class="sxs-lookup"><span data-stu-id="6d990-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="6d990-107">Este un simbol web JSON (JWT) emis special către tokenul de la prima parte Microsoft, pentru a activa sign-on unic (SSO) în aplicațiile utilizate pe aceste dispozitive.</span><span class="sxs-lookup"><span data-stu-id="6d990-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="6d990-108">În Ce este un token de reîmprospătare [principal?,](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)vom oferi detalii despre modul în care un PRT este emis, utilizat și protejat pe dispozitivele Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6d990-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="6d990-109">**WamDefaultSet: YES și AzureADPrt: DA** Aceste câmpuri indică dacă utilizatorul s-a autentificat cu succes la Azure AD atunci când s-a conectat la dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="6d990-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="6d990-110">Dacă valorile sunt **NU,** este posibil ca aceasta să fie scadentă:</span><span class="sxs-lookup"><span data-stu-id="6d990-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="6d990-111">Cheie de stocare nereparticulară în TPM asociată cu dispozitivul după înregistrare (verificați KeySignTest în timp ce rulează cu nivel ridicat).</span><span class="sxs-lookup"><span data-stu-id="6d990-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="6d990-112">ID conectare alternativă</span><span class="sxs-lookup"><span data-stu-id="6d990-112">Alternate Login ID</span></span>
- <span data-ttu-id="6d990-113">Proxy HTTP nu a fost găsit</span><span class="sxs-lookup"><span data-stu-id="6d990-113">HTTP Proxy not found</span></span>

<span data-ttu-id="6d990-114">Depanarea dispozitivelor utilizând comanda dsregcmd - [starea SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="6d990-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
