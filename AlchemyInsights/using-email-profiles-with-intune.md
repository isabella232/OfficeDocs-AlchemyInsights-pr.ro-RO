---
title: Utilizarea profilurilor de e-mail cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653300"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="19d2e-102">Utilizarea profilurilor de e-mail cu Intune</span><span class="sxs-lookup"><span data-stu-id="19d2e-102">Using email profiles with Intune</span></span>

<span data-ttu-id="19d2e-103">Intune poate fi utilizat pentru a crea și implementa profiluri de e-mail pentru clientul de e-mail nativ (încorporat) de pe mai multe platforme de dispozitive.</span><span class="sxs-lookup"><span data-stu-id="19d2e-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="19d2e-104">Pentru informații despre unele dintre restricțiile asociate cu profilurile de e-mail, inclusiv despre modul în care sunt gestionate prezența profilurilor existente și cum să eliminați profilurile de e-mail, consultați [adăugarea setărilor de e-mail la dispozitivele care utilizează Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="19d2e-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="19d2e-105">Pentru mai multe informații despre cum să creați profiluri de e-mail pentru fiecare platformă de dispozitive, consultați:</span><span class="sxs-lookup"><span data-stu-id="19d2e-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="19d2e-106">Setări dispozitiv Android pentru a configura e-mailul, autentificarea și sincronizarea în Intune</span><span class="sxs-lookup"><span data-stu-id="19d2e-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="19d2e-107">Adăugarea setărilor de e-mail pentru dispozitive iOS și iPadOS în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="19d2e-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="19d2e-108">Setările de profil de e-mail din Microsoft Intune pentru dispozitivele care execută Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="19d2e-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="19d2e-109">Setările de profil de e-mail pentru dispozitivele care execută Windows 10 în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="19d2e-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="19d2e-110">**Problemă de sincronizare obișnuită**</span><span class="sxs-lookup"><span data-stu-id="19d2e-110">**Common syncing issue**</span></span>

<span data-ttu-id="19d2e-111">**Un KNOX din profilul de e-mail Android previne persoanele de contact, calendarul și activitățile de utilizator, de la sincronizarea la dispozitivele de utilizator.**</span><span class="sxs-lookup"><span data-stu-id="19d2e-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="19d2e-112">Profilul de e-mail KNOX din Android KNOX oferă administratorului opțiunea de a decide ce tipuri de conținut sunt sincronizate cu dispozitivul setând fiecare la activat.</span><span class="sxs-lookup"><span data-stu-id="19d2e-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="19d2e-113">Dacă setarea pentru oricare dintre tipurile de conținut este setată la **neconfigurat** (implicit), acel tip de conținut nu se sincronizează automat.</span><span class="sxs-lookup"><span data-stu-id="19d2e-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="19d2e-114">Un utilizator poate activa tipul de conținut pe care îl doresc direct pe dispozitiv, dar acea configurație este suprascrisă de setarea de politică Intune, iar sincronizarea se oprește pentru acel tip de conținut.</span><span class="sxs-lookup"><span data-stu-id="19d2e-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

