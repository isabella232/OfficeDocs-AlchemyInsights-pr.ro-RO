---
title: Utilizați liniile de bază de securitate Microsoft Intune pentru a configura dispozitivele Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696379"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="d8b1b-102">Utilizați liniile de bază de securitate Microsoft Intune pentru configurarea dispozitivelor Windows 10</span><span class="sxs-lookup"><span data-stu-id="d8b1b-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="d8b1b-103">Liniile de referință de securitate Intune ajută la protejarea utilizatorilor și dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="d8b1b-104">Liniile de referință de securitate sunt grupuri de setări Windows preconfigurate utilizate pentru a aplica un grup cunoscut de setări și valori implicite recomandate de echipele de securitate relevante.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="d8b1b-105">Prin crearea unui profil de referință de securitate în Intune, creați un șablon care constă din mai multe profiluri de configurare a dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="d8b1b-106">Atunci când implementați linii de referință de securitate la grupuri de utilizatori sau dispozitive, setările se aplică la dispozitivele care rulează în Windows 10 sau versiuni mai recente.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="d8b1b-107">De exemplu, linia de bază de securitate Microsoft Mobile Device Management (MDM) activează automat (1) activează BitLocker pentru unitățile amovibile, (2) necesită parola pentru deblocarea unui dispozitiv și (3) dezactivează autentificarea de bază.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="d8b1b-108">Atunci când o valoare implicită nu funcționează pentru mediul dvs., puteți particulariza valoarea de referință pentru a aplica setările de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="d8b1b-109">De asemenea, liniile de referință de securitate vă ajută să stabiliți un flux de lucru securizat final în Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="d8b1b-110">Iată câteva avantaje ale acestei funcționalități:</span><span class="sxs-lookup"><span data-stu-id="d8b1b-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="d8b1b-111">O linie de bază de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="d8b1b-112">Deoarece Intune parteneri cu echipa de securitate Windows care creează valori de referință pentru politicile de grup, aceste recomandări se bazează pe orientări solide și o experiență extinsă.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="d8b1b-113">Dacă nu sunteți familiarizat cu Intune și nu sunteți sigur de unde să începeți, atunci liniile de referință de securitate vă vor ajuta să creați și să implementați rapid un profil securizat.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="d8b1b-114">Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai simplă cu liniile de bază de securitate, deoarece aceste linii de referință de securitate sunt încorporate în Intune și includ capacități de vârf pentru gestionare.</span><span class="sxs-lookup"><span data-stu-id="d8b1b-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="d8b1b-115">Pentru mai multe informații, consultați [liniile de bază de securitate Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) și [gestionarea dispozitivelor mobile](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="d8b1b-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>