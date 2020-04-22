---
title: Termeni care lipsesc din Depozitul de termeni SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766865"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="e72ce-102">Activarea criptării Bitlocker cu Intune</span><span class="sxs-lookup"><span data-stu-id="e72ce-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="e72ce-103">Intune Endpoint Protection Policy poate fi utilizat pentru a configura setările de criptare Boitlocker pentru dispozitiveLe Windows, așa este descris în: Setări Windows10 (și versiuni ulterioare) pentru a proteja dispozitivele utilizând Intune</span><span class="sxs-lookup"><span data-stu-id="e72ce-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="e72ce-104">Ar trebui să fie conștienți de faptul că multe dispozitive mai noi care execută Windows 10 acceptă criptarea automată bitlocker care se declanșează fără aplicarea politicii MDM.</span><span class="sxs-lookup"><span data-stu-id="e72ce-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="e72ce-105">Acest lucru poate avea impact asupra aplicării politicii dacă sunt configurate setările neimplicite.</span><span class="sxs-lookup"><span data-stu-id="e72ce-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="e72ce-106">Consultați Întrebări frecvente pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="e72ce-106">See FAQ for more detail.</span></span>


<span data-ttu-id="e72ce-107">Faq  Î: Ce ediții de criptare dispozitiv de asistență Windows utilizând Politica de protecție Endpoint?</span><span class="sxs-lookup"><span data-stu-id="e72ce-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="e72ce-108"> R: Setările din Intune Endpoint Protection Policy sunt implementate utilizând Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="e72ce-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="e72ce-109">Nu toate edițiile, nici compilările de Windows acceptă Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="e72ce-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="e72ce-110">În acest moment Edițiile Windows: Enterprise; Sunt acceptate educația, mobilul, întreprinderea mobilă și profesioniștii (începând cu versiunea 1809).</span><span class="sxs-lookup"><span data-stu-id="e72ce-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="e72ce-111">Î: Dacă un dispozitiv este deja criptat cu Bitlocker utilizând setările implicite ale sistemului de operare pentru metoda de criptare și puterea de criptare (XTS-AES-128) aplicarea unei politici cu setări diferite declanșează automat recriptarea unității cu noile setări?</span><span class="sxs-lookup"><span data-stu-id="e72ce-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="e72ce-112">R: Nu.</span><span class="sxs-lookup"><span data-stu-id="e72ce-112">A: No.</span></span> <span data-ttu-id="e72ce-113">Pentru a aplica noile setări de cifru, unitatea trebuie mai întâi decriptată.</span><span class="sxs-lookup"><span data-stu-id="e72ce-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="e72ce-114">Notă Pentru dispozitivele înscrise cu Autopilot criptarea automată care ar apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată, care permite setările bazate pe politică pentru a fi utilizate în loc de valori implicite os</span><span class="sxs-lookup"><span data-stu-id="e72ce-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="e72ce-115">Q Dacă un dispozitiv este criptat ca urmare a aplicării politicii Intune va fi decriptat atunci când această politică este eliminat?</span><span class="sxs-lookup"><span data-stu-id="e72ce-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="e72ce-116">R: Eliminarea politicii legate de criptare NU duce la decriptarea unităților care au fost configurate.</span><span class="sxs-lookup"><span data-stu-id="e72ce-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="e72ce-117">Î: De ce politica de conformitate intune arată că dispozitivul meu nu are "Bitlocker Activat", dar este?</span><span class="sxs-lookup"><span data-stu-id="e72ce-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="e72ce-118">R: Setarea "Bitlocker activat" în politica de conformitate intune utilizează clientul Windows Device Health Atestare (DHA).</span><span class="sxs-lookup"><span data-stu-id="e72ce-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="e72ce-119">Acest client măsoară numai starea dispozitivului la momentul pornire.</span><span class="sxs-lookup"><span data-stu-id="e72ce-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="e72ce-120">Deci, dacă un dispozitiv nu a fost repornit, deoarece criptarebitlocker a fost finalizat serviciul client DHA nu va raporta bitlocker ca fiind activ.</span><span class="sxs-lookup"><span data-stu-id="e72ce-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>