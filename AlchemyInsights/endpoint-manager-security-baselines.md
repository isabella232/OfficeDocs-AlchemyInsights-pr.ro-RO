---
title: EndPoint Manager - Referințe de securitate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421088"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="04254-102">EndPoint Manager - Referințe de securitate</span><span class="sxs-lookup"><span data-stu-id="04254-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="04254-103">Nivelurile de referință de securitate sunt grupuri preconfigurate de setări Windows care vă ajută să aplicați setările de securitate recomandate de echipele de securitate relevante.</span><span class="sxs-lookup"><span data-stu-id="04254-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="04254-104">Aceste niveluri de referință pot fi particularizate pentru a livra doar setările și valorile dorite.</span><span class="sxs-lookup"><span data-stu-id="04254-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="04254-105">Pentru mai multe informații despre nivelurile de referință de securitate, consultați Utilizarea nivelurilor de referință de securitate pentru a [configura dispozitivele Windows 10 în Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="04254-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="04254-106">În prezent, există niveluri de referință pentru aceste produse:</span><span class="sxs-lookup"><span data-stu-id="04254-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="04254-107">Setări Securitate Windows MDM</span><span class="sxs-lookup"><span data-stu-id="04254-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="04254-108">Microsoft Defender pentru securitatea punct final</span><span class="sxs-lookup"><span data-stu-id="04254-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="04254-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="04254-109">Microsoft Edge</span></span>

<span data-ttu-id="04254-110">Fiecare dintre referințe este actualizată periodic și lansată în versiuni incrementale.</span><span class="sxs-lookup"><span data-stu-id="04254-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="04254-111">Fiecare versiune adaugă și sau elimină setările din versiunea anterioară pentru a se asigura că linia de referință îndeplinește instrucțiunile curente.</span><span class="sxs-lookup"><span data-stu-id="04254-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="04254-112">Consola De referință de securitate din Securitatea punctelor finale permite compararea diferitelor versiuni, făcând vizibile modificările de la o versiune la alta.</span><span class="sxs-lookup"><span data-stu-id="04254-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="04254-113">Pentru instrucțiuni despre cum să modificați cât mai eficient ce versiune de referință este implementată, consultați Gestionarea profilurilor de linie de referință de [securitate în Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="04254-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="04254-114">După implementarea unui nivel de referință de securitate, puteți să monitorizați starea implementării și să revizuiți setările pe dispozitive.</span><span class="sxs-lookup"><span data-stu-id="04254-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="04254-115">**Notă:** Datele de raportare pentru nivelurile de referință pot dura până la 24 de ore pentru a apărea din implementarea inițială pe un dispozitiv și până la 6 ore pentru actualizări suplimentare.</span><span class="sxs-lookup"><span data-stu-id="04254-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="04254-116">Cauza cea mai comună a unei setări de referință care nu se aplică este faptul că aceeași setare este utilizată în alt profil.</span><span class="sxs-lookup"><span data-stu-id="04254-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="04254-117">Acest scenariu poate fi investigat pentru un anumit dispozitiv, selectând acel dispozitiv din nodul Stare dispozitiv al profilului de referință de securitate.</span><span class="sxs-lookup"><span data-stu-id="04254-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="04254-118">Pentru detalii, consultați [Rezolvarea conflictelor pentru nivelurile de referință de securitate](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="04254-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>