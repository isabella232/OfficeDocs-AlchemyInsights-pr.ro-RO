---
title: Regulile de reducere a suprafeței de atac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676440"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c8672-102">Regulile de reducere a suprafeței de atac</span><span class="sxs-lookup"><span data-stu-id="c8672-102">Attack surface reduction rules</span></span>

<span data-ttu-id="c8672-103">Excluderea fișierelor sau folderelor poate reduce grav protecția oferită de regulile de reducere a suprafeței de atac.</span><span class="sxs-lookup"><span data-stu-id="c8672-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="c8672-104">Fișierele care ar fi fost blocate de o regulă au permisiunea de a rula și nu este înregistrat niciun raport sau eveniment.</span><span class="sxs-lookup"><span data-stu-id="c8672-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="c8672-105">Excluderea se aplică tuturor regulilor care permit excluderi.</span><span class="sxs-lookup"><span data-stu-id="c8672-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="c8672-106">Excluderile ASR utilizează aceeași sintaxă ca Antivirus Microsoft Defender excluderile.</span><span class="sxs-lookup"><span data-stu-id="c8672-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="c8672-107">Pentru detalii, consultați [Configurarea și validarea excluderilor pentru Antivirus Microsoft Defender scanare.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c8672-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="c8672-108">Pentru a evita problemele, [revizuiți Greșelile comune de evitat atunci când definiți excluderi.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c8672-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c8672-109">Nu toate regulile ASR acceptă excluderile.</span><span class="sxs-lookup"><span data-stu-id="c8672-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="c8672-110">Pentru a valida dacă regula dvs. acceptă excluderi, consultați tabelul Regulile de [reducere a suprafeței de atac.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c8672-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c8672-111">Regulile de reducere a suprafeței de atac</span><span class="sxs-lookup"><span data-stu-id="c8672-111">Attack surface reduction rules</span></span>

<span data-ttu-id="c8672-112">Suprafața de atac a organizației dvs. include toate locurile unde un atacant ar putea compromite dispozitivele sau rețelele organizației.</span><span class="sxs-lookup"><span data-stu-id="c8672-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="c8672-113">Reducerea suprafeței de atac înseamnă protejarea dispozitivelor organizației și a rețelei, ceea ce lasă atacurile cu mai puține modalități de a efectua atacuri.</span><span class="sxs-lookup"><span data-stu-id="c8672-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="c8672-114">Configurarea regulilor de reducere a suprafeței de atac în Microsoft Defender pentru punctul final vă poate ajuta.</span><span class="sxs-lookup"><span data-stu-id="c8672-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="c8672-115">Pentru mai multe informații, consultați:</span><span class="sxs-lookup"><span data-stu-id="c8672-115">For more information, see:</span></span>

- [<span data-ttu-id="c8672-116">Mapare GUID pentru regula ASR pentru nume</span><span class="sxs-lookup"><span data-stu-id="c8672-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="c8672-117">Cerințe de reguli ASR:</span><span class="sxs-lookup"><span data-stu-id="c8672-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="c8672-118">Windows 10 Pro, versiunea 1709 sau o versiune mai recentă</span><span class="sxs-lookup"><span data-stu-id="c8672-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c8672-119">Windows 10 Enterprise, versiunea 1709 sau o versiune mai recentă</span><span class="sxs-lookup"><span data-stu-id="c8672-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c8672-120">Windows Server, versiunea 1803 (Canalul semi-anual) sau o versiune mai recentă</span><span class="sxs-lookup"><span data-stu-id="c8672-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="c8672-121">Identificați excluderea corectă de aplicat</span><span class="sxs-lookup"><span data-stu-id="c8672-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="c8672-122">Căutați eventID 1121 sau 1122 în jurnalul Microsoft-Windows-Windows Defender/operațional.</span><span class="sxs-lookup"><span data-stu-id="c8672-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="c8672-123">Evaluați scenariul și contextul blocului și confirmați că acest scenariu trebuie deblocat.</span><span class="sxs-lookup"><span data-stu-id="c8672-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="c8672-124">Citiți valoarea Cale din detaliile evenimentului, care este valoarea care definește excluderea.</span><span class="sxs-lookup"><span data-stu-id="c8672-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="c8672-125">Faceți excluderea cât mai strictă posibil.</span><span class="sxs-lookup"><span data-stu-id="c8672-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="c8672-126">Aplicați un wildcard acolo unde este necesar (de exemplu, înlocuiți variabila utilizator).</span><span class="sxs-lookup"><span data-stu-id="c8672-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="c8672-127">Aplicați excluderea în funcție de nevoile dvs. de implementare.</span><span class="sxs-lookup"><span data-stu-id="c8672-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="c8672-128">Pentru detalii, consultați Particularizarea [regulilor de reducere a suprafeței de atac.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="c8672-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="c8672-129">Excluderea nu este onorată</span><span class="sxs-lookup"><span data-stu-id="c8672-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="c8672-130">Determinați dacă regula acceptă excluderi.</span><span class="sxs-lookup"><span data-stu-id="c8672-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="c8672-131">Pentru detalii, consultați Regulile [de reducere a suprafeței de atac.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c8672-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="c8672-132">Revizuiți excluderile aplicate și verificați cu datele evenimentului dacă există metacaractere tastare sau interpretate greșit.</span><span class="sxs-lookup"><span data-stu-id="c8672-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="c8672-133">Pentru mai multe informații, consultați [Tipuri de excluderi acceptate](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="c8672-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="c8672-134">dacă impactul regulii este prea mare, luați în considerare mutarea regulii (înapoi) în Modul auditare pentru a efectua validări suplimentare.</span><span class="sxs-lookup"><span data-stu-id="c8672-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="c8672-135">Pentru detalii, consultați [Testarea modului în care funcționează caracteristicile Microsoft Defender pentru puncte finale în modul de auditare.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="c8672-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="c8672-136">Colectați date de asistență pentru a deschide un caz de asistență utilizând această comandă:</span><span class="sxs-lookup"><span data-stu-id="c8672-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="c8672-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="c8672-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="c8672-138">Pentru mai multe informații, [consultați Probleme cu mașinile de bord la Microsoft Defender pentru puncte finale.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="c8672-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
