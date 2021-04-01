---
title: Manager Punct final - Niveluri de referință pentru securitate
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440896"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="2ff89-102">Manager Punct final - Niveluri de referință pentru securitate</span><span class="sxs-lookup"><span data-stu-id="2ff89-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="2ff89-103">Nivelurile de referință pentru securitate sunt grupuri preconfigurate de setări Windows care vă ajută să aplicați setările de securitate recomandate de echipele de securitate relevante.</span><span class="sxs-lookup"><span data-stu-id="2ff89-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="2ff89-104">Aceste niveluri de referințe pot fi particularizate pentru a livra doar setările și valorile dorite.</span><span class="sxs-lookup"><span data-stu-id="2ff89-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="2ff89-105">Pentru mai multe informații despre nivelurile de referință pentru securitate, consultați [Utilizați niveluri de referință pentru securitate pentru a configura dispozitivele Windows 10 în Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="2ff89-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="2ff89-106">Există niveluri de referință pentru aceste produse:</span><span class="sxs-lookup"><span data-stu-id="2ff89-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="2ff89-107">Setări de securitate MDM Windows</span><span class="sxs-lookup"><span data-stu-id="2ff89-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="2ff89-108">Microsoft Defender pentru securitate Punct final</span><span class="sxs-lookup"><span data-stu-id="2ff89-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="2ff89-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2ff89-109">Microsoft Edge</span></span>

<span data-ttu-id="2ff89-110">Fiecare dintre nivelurile de referință este actualizat periodic și lansat în versiuni incrementale.</span><span class="sxs-lookup"><span data-stu-id="2ff89-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="2ff89-111">Fiecare versiune adaugă și elimină setările din versiunea anterioară, pentru a se asigura că nivelul de referință îndeplinește instrucțiunile actuale.</span><span class="sxs-lookup"><span data-stu-id="2ff89-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="2ff89-112">Consola cu niveluri de referință de securitate din Securitatea punctului final permite compararea diferitelor versiuni, făcând vizibile modificările de la o versiune la alta.</span><span class="sxs-lookup"><span data-stu-id="2ff89-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="2ff89-113">Pentru instrucțiuni despre cum să modificați eficient versiunea nivelului de referință implementată, consultați [Gestionarea profilurilor privind nivelul de referință de securitate în Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="2ff89-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="2ff89-114">După implementarea unui nivel de referință pentru securitate, puteți monitoriza starea setărilor de implementare și revizuire pe o bază de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="2ff89-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="2ff89-115">**Notă:** Datele de raportare pentru nivelurile de referință pot dura până la 24 de ore pentru a apărea de la implementarea inițială pe un dispozitiv și până la 6 ore pentru actualizări suplimentare.</span><span class="sxs-lookup"><span data-stu-id="2ff89-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="2ff89-116">Cauza cea mai comună a neaplicării unei setări a nivelului de referință este faptul că aceeași setare este utilizată în alt profil.</span><span class="sxs-lookup"><span data-stu-id="2ff89-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="2ff89-117">Acest scenariu poate fi investigat pentru un anumit dispozitiv selectând acel dispozitiv din nodul Stare dispozitiv al profilului Nivel de referință pentru securitate.</span><span class="sxs-lookup"><span data-stu-id="2ff89-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="2ff89-118">Pentru detalii, consultați [Soluționarea conflictelor privind referințele pentru securitate](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="2ff89-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>