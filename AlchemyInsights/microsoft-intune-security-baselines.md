---
title: Utilizați Microsoft Intune de referință de securitate pentru a configura Windows 10 dispozitive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793892"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="3d007-102">Utilizați Microsoft Intune de referință de securitate pentru a configura Windows 10 dispozitive</span><span class="sxs-lookup"><span data-stu-id="3d007-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="3d007-103">Nivelurile de referință de securitate Intune contribuie la protejarea utilizatorilor și a dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="3d007-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="3d007-104">Referințele de Windows sunt grupurile preconfigurate utilizate pentru a aplica un grup cunoscut de setări și valorile implicite recomandate de echipele de securitate relevante.</span><span class="sxs-lookup"><span data-stu-id="3d007-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="3d007-105">Creând un profil de referință de securitate în Intune, creați un șablon care constă în mai multe profiluri de configurare a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="3d007-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="3d007-106">Atunci când implementați niveluri de referință de securitate pentru grupuri de utilizatori sau dispozitive, setările se aplică pentru dispozitivele care rulează pe dispozitivele Windows 10 sau mai recente.</span><span class="sxs-lookup"><span data-stu-id="3d007-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="3d007-107">De exemplu, nivelul de referință de securitate MDM (mobile device management) Microsoft activează automat BitLocker pentru unitățile amovibile, necesită parola pentru deblocarea unui dispozitiv și dezactivează autentificarea de bază.</span><span class="sxs-lookup"><span data-stu-id="3d007-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="3d007-108">Atunci când o valoare implicită nu funcționează pentru mediul dvs., puteți particulariza nivelul de referință pentru a aplica setările de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="3d007-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="3d007-109">De asemenea, referințele de securitate vă ajută să stabiliți un flux de lucru securizat end-to-end Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3d007-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="3d007-110">Un nivel de referință de securitate include cele mai bune practici și recomandări pentru setările care afectează securitatea.</span><span class="sxs-lookup"><span data-stu-id="3d007-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="3d007-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based solid guidance and extensive experience.</span><span class="sxs-lookup"><span data-stu-id="3d007-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="3d007-112">Dacă nu sunteți sigur de unde să începeți, nivelurile de referință de securitate vă ajută să creați și să implementați rapid un profil sigur.</span><span class="sxs-lookup"><span data-stu-id="3d007-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="3d007-113">Dacă utilizați în prezent o politică de grup, migrarea la Intune în scopuri de gestionare este mult mai ușoară cu nivelurile de referință de securitate, deoarece acestea sunt încorporate în Intune și includ capacități de gestionare de ultimă oră.</span><span class="sxs-lookup"><span data-stu-id="3d007-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="3d007-114">Pentru a afla mai multe, [consultați Referințe Windows securitate și](/windows/security/threat-protection/windows-security-baselines) Gestionarea [dispozitivelor mobile.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="3d007-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

