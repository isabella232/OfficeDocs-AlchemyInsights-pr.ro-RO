---
title: Profiluri Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555318"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="6abf9-102">Profiluri Wi-Fi Intune</span><span class="sxs-lookup"><span data-stu-id="6abf9-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="6abf9-103">Implementarea cu succes a conectivității Wi-Fi pentru clienții MDM depinde de un profil implementat corect, care reflectă cerințele infrastructurii Wi-Fi corporative.</span><span class="sxs-lookup"><span data-stu-id="6abf9-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="6abf9-104">Pentru a examina setările corespunzătoare pentru platformele client pe care le investigați, consultați:</span><span class="sxs-lookup"><span data-stu-id="6abf9-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="6abf9-105">Adăugarea setărilor Wi-Fi pentru dispozitivele care rulează Android în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6abf9-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="6abf9-106">Adăugarea setărilor Wi-Fi pentru dispozitivele dedicate și gestionate de Android Enterprise în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6abf9-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="6abf9-107">Adăugarea setărilor Wi-Fi pentru dispozitivele iOS și iPadOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6abf9-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="6abf9-108">Adăugarea setărilor Wi-Fi pentru Windows 10 și dispozitivele ulterioare în Intune</span><span class="sxs-lookup"><span data-stu-id="6abf9-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="6abf9-109">Importul setărilor Wi-Fi pentru dispozitivele Windows în Intune</span><span class="sxs-lookup"><span data-stu-id="6abf9-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="6abf9-110">**Probleme comune**</span><span class="sxs-lookup"><span data-stu-id="6abf9-110">**Common Issues**</span></span>

<span data-ttu-id="6abf9-111">**Implementez un profil Wi-Fi care depinde de un certificat implementat specificat în profilul Wi-Fi. Cu toate acestea, profilurile de configurare afișează o stare de eroare.**</span><span class="sxs-lookup"><span data-stu-id="6abf9-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="6abf9-112">Verificați dacă dispozitivul a primit certificatul.</span><span class="sxs-lookup"><span data-stu-id="6abf9-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="6abf9-113">În Intune, accesați **Toate dispozitivele** și selectați dispozitivul > **configurația dispozitivului**.</span><span class="sxs-lookup"><span data-stu-id="6abf9-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="6abf9-114">Verificați dacă toate profilurile așteptate sunt listate și într-o stare de succes.</span><span class="sxs-lookup"><span data-stu-id="6abf9-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="6abf9-115">Pentru un profil Android, dacă aveți certificate intermediare în lanțul de certificate, asigurați-vă că acestea sunt implementate pe dispozitive Android.</span><span class="sxs-lookup"><span data-stu-id="6abf9-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="6abf9-116">Pentru a verifica starea certificatului, accesați Profiluri **de configurare dispozitiv**Android intermediar  >  **Profiles**  >  **CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="6abf9-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="6abf9-117">Dacă continuați să vedeți erori, examinați procedurile și secțiunile de depanare.</span><span class="sxs-lookup"><span data-stu-id="6abf9-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="6abf9-118">Pentru mai multe informații, consultați [Prezentare generală pentru depanarea profilurilor de certificate SCEP cu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="6abf9-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="6abf9-119">**Am implementat un profil Wi-Fi pe un dispozitiv. Intune arată că a avut succes, dar dispozitivul nu se conectează la Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="6abf9-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="6abf9-120">O stare reușită înseamnă că Intune a implementat cu succes profilul așa a fost configurat.</span><span class="sxs-lookup"><span data-stu-id="6abf9-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="6abf9-121">Cu toate acestea, este posibil ca aceste configurații să nu corespundă cerințelor de rețea și/sau autentificare.</span><span class="sxs-lookup"><span data-stu-id="6abf9-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="6abf9-122">Pentru mai multe detalii despre tentativa de conectare, examinați jurnalele din serviciul de infrastructură și autentificare (pe controlerul punctului de acces Wi-Fi și pe serverul NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="6abf9-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="6abf9-123">Poate fi necesar să lucrați cu echipa de infrastructură de rețea sau cu furnizorul terț de Wi-Fi pentru a aduna și a revizui jurnalele.</span><span class="sxs-lookup"><span data-stu-id="6abf9-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>