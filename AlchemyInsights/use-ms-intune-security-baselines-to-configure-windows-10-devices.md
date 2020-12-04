---
title: Utilizați liniile de bază de securitate Microsoft Intune pentru a configura dispozitivele Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573533"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="f56c0-102">Utilizați liniile de bază de securitate Microsoft Intune pentru a configura dispozitivele Windows 10</span><span class="sxs-lookup"><span data-stu-id="f56c0-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="f56c0-103">Liniile de referință de securitate Intune ajută la protejarea utilizatorilor și dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="f56c0-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="f56c0-104">Liniile de referință de securitate sunt grupuri de setări Windows preconfigurate utilizate pentru a aplica un grup cunoscut de setări și valori implicite recomandate de echipele de securitate relevante.</span><span class="sxs-lookup"><span data-stu-id="f56c0-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="f56c0-105">Prin crearea unui profil de referință de securitate în Intune, creați un șablon care constă din mai multe profiluri de configurare a dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="f56c0-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="f56c0-106">Atunci când implementați linii de referință de securitate la grupuri de utilizatori sau dispozitive, setările se aplică la dispozitivele care rulează în Windows 10 sau o versiune mai recentă.</span><span class="sxs-lookup"><span data-stu-id="f56c0-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="f56c0-107">De exemplu, linie de bază de securitate MDM automat (1) activează BitLocker pentru unitățile amovibile, (2) necesită parola pentru deblocarea unui dispozitiv și (3) dezactivează autentificarea de bază.</span><span class="sxs-lookup"><span data-stu-id="f56c0-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="f56c0-108">Atunci când o valoare implicită nu funcționează pentru mediul dvs., particularizați valoarea de referință pentru a aplica setările de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="f56c0-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="f56c0-109">De asemenea, liniile de referință de securitate vă ajută să stabiliți un flux de lucru securizat final în Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f56c0-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="f56c0-110">Iată câteva dintre următoarele avantaje:</span><span class="sxs-lookup"><span data-stu-id="f56c0-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="f56c0-111">O linie de bază de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea.</span><span class="sxs-lookup"><span data-stu-id="f56c0-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="f56c0-112">Deoarece Intune parteneri cu echipa de securitate Windows care creează valori de referință pentru politicile de grup, aceste recomandări se bazează pe orientări solide și o experiență extinsă.</span><span class="sxs-lookup"><span data-stu-id="f56c0-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="f56c0-113">Dacă nu sunteți familiarizat cu Intune și nu sunteți sigur de unde să începeți, atunci liniile de referință de securitate vă vor ajuta să creați și să implementați rapid un profil securizat.</span><span class="sxs-lookup"><span data-stu-id="f56c0-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="f56c0-114">Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai simplă cu liniile de bază de securitate, deoarece acestea sunt încorporate în Intune și includ capacități de vârf pentru gestionare.</span><span class="sxs-lookup"><span data-stu-id="f56c0-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="f56c0-115">Pentru a afla mai multe, consultați [liniile de bază de securitate Windows](https://go.microsoft.com/fwlink/?linkid=2141503) și [gestionarea dispozitivelor mobile](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="f56c0-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>