---
title: Probleme legate de VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555229"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="fe4d7-102">Probleme legate de VPN</span><span class="sxs-lookup"><span data-stu-id="fe4d7-102">VPN related issues</span></span>

<span data-ttu-id="fe4d7-103">Implementarea cu succes a conectivității VPN pentru clienții MDM depinde de un profil implementat care reflectă corect cerințele infrastructurii VPN.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="fe4d7-104">Pentru setările corespunzătoare pentru platformele client pe care le investigați, consultați:</span><span class="sxs-lookup"><span data-stu-id="fe4d7-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="fe4d7-105">Setările dispozitivelor holografice Windows 10 și Windows pentru a adăuga conexiuni VPN utilizând Intune</span><span class="sxs-lookup"><span data-stu-id="fe4d7-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="fe4d7-106">Adăugarea setărilor VPN pe dispozitivele iOS și iPadOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fe4d7-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="fe4d7-107">Setările dispozitivului Android pentru a configura VPN în Intune</span><span class="sxs-lookup"><span data-stu-id="fe4d7-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="fe4d7-108">Adăugarea setărilor VPN pe dispozitivele macOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fe4d7-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="fe4d7-109">Dacă profilul VPN utilizează autentificarea bazată pe certificat, asigurați-vă că profilurile de certificat de certificat rădăcină și de autentificare client legate la profilul VPN sunt implementate cu succes.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="fe4d7-110">**Probleme comune**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-110">**Common Issues**</span></span>

<span data-ttu-id="fe4d7-111">**Am implementat un profil VPN pe un dispozitiv. Intune arată că a avut succes, dar dispozitivul nu se conectează la VPN.**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="fe4d7-112">O stare reușită înseamnă că Intune a implementat cu succes profilul așa a fost configurat.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="fe4d7-113">Cu toate acestea, este posibil ca aceste configurații să nu corespundă cerințelor de rețea și/sau autentificare.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="fe4d7-114">Examinați jurnalele din serviciul de infrastructură și autentificare (pe serverul VPN și serverul NPS/Radius) pentru mai multe detalii despre a încercat conexiunea.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="fe4d7-115">Poate fi necesar să lucrați cu echipa de infrastructură de rețea sau cu furnizorul VPN terț pentru a colecta și a revizui jurnalele.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="fe4d7-116">**Când configurez un VPN personalizat pentru iOS, funcția VPN per aplicație nu este disponibilă.**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="fe4d7-117">VPN per aplicație pentru dispozitivele iOS din Intune este disponibil în prezent pentru o anumită listă de furnizori și parteneri, care trebuie să îndeplinească, de asemenea, cerințele preliminare ale certificatului înainte de a configura un VPN per aplicație.</span><span class="sxs-lookup"><span data-stu-id="fe4d7-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="fe4d7-118">Pentru mai multe informații, consultați [Configurarea rețelei private virtuale (VPN) per aplicație pentru dispozitivele iOS/iPadOS în Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="fe4d7-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="fe4d7-119">Pentru mai multe informații despre toate tipurile de conexiuni VPN din Intune, consultați [Crearea profilurilor VPN pentru conectarea la serverele VPN din Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="fe4d7-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="fe4d7-120">**VPN la cerere iOS nu se declanșează atunci când este accesat un domeniu configurat**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="fe4d7-121">Pentru a testa setările VPN automate, setați următoarele valori:</span><span class="sxs-lookup"><span data-stu-id="fe4d7-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="fe4d7-122">Doresc să fac următoarele: **Evaluați fiecare încercare de conectare**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="fe4d7-123">Alegeți dacă să vă conectați: **Conectați-vă dacă este necesar**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="fe4d7-124">Când utilizatorii accesează aceste domenii: *nume de domeniu* **țintă**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="fe4d7-125">Dacă configurația de mai sus nu reușește, adăugați următorul element:</span><span class="sxs-lookup"><span data-stu-id="fe4d7-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="fe4d7-126">Când acest URL este inaccesibil, forțați conectarea VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="fe4d7-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>