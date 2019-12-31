---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908721"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="4246e-102">Activarea criptare BitLocker cu Intune</span><span class="sxs-lookup"><span data-stu-id="4246e-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="4246e-103">Intune Endpoint Protection politica poate fi utilizat pentru a configura setările de criptare BitLocker pentru dispozitive Windows.</span><span class="sxs-lookup"><span data-stu-id="4246e-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="4246e-104">Pentru mai multe informații, consultați [setările Windows 10 (și versiunile ulterioare) pentru a proteja dispozitivele care utilizează Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="4246e-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="4246e-105">Ar trebui să știți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată BitLocker, care este declanșată fără aplicarea politicii MDM.</span><span class="sxs-lookup"><span data-stu-id="4246e-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="4246e-106">Acest lucru poate afecta aplicarea politicii dacă sunt configurate Setări non-implicite.</span><span class="sxs-lookup"><span data-stu-id="4246e-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="4246e-107">Consultați următoarele întrebări frecvente pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="4246e-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="4246e-108">Pentru informații despre depanarea problemelor cu BitLocker, consultați [Depanarea politicilor BitLocker în Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="4246e-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="4246e-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="4246e-109">**FAQ**</span></span>

 <span data-ttu-id="4246e-110">Q: ce ediții de criptare dispozitiv de suport Windows utilizând politica de protecție Endpoint?</span><span class="sxs-lookup"><span data-stu-id="4246e-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="4246e-111">A: setările din Intune Endpoint Politica de protecție sunt implementate utilizând CSP-ul [BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="4246e-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="4246e-112">Nu toate edițiile sau compilările de Windows acceptă CSP-ul BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4246e-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="4246e-113">În acest moment, sunt acceptate următoarele ediții Windows: Enterprise, Education, mobile, Mobile Enterprise și Professional (compilare 1809 și versiuni ulterioare).</span><span class="sxs-lookup"><span data-stu-id="4246e-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="4246e-114">Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite ale sistemului de operare pentru metoda de criptare și puterea cifrului (XTS-AES-128), va aplica o politică cu diferite setări declanșează automat re-criptarea unității cu noile setări?</span><span class="sxs-lookup"><span data-stu-id="4246e-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="4246e-115">A: nu.</span><span class="sxs-lookup"><span data-stu-id="4246e-115">A: No.</span></span> <span data-ttu-id="4246e-116">Pentru a aplica noile setări de cifrare, unitatea trebuie mai întâi decriptată.</span><span class="sxs-lookup"><span data-stu-id="4246e-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="4246e-117">**Notă:** Pentru dispozitivele care se înscriu cu autopilot, criptarea automată care ar apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată, care permite setările bazate pe politici pentru a fi utilizate în locul implicite de sistem de operare.</span><span class="sxs-lookup"><span data-stu-id="4246e-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="4246e-118">Î: dacă un dispozitiv este criptat ca urmare a aplicării politicii Intune, va fi decriptat atunci când această politică este eliminată?</span><span class="sxs-lookup"><span data-stu-id="4246e-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="4246e-119">A: eliminarea politicii legate de criptare nu duce la decriptarea unităților care au fost configurate.</span><span class="sxs-lookup"><span data-stu-id="4246e-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="4246e-120">Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are BitLocker activat, chiar dacă este?</span><span class="sxs-lookup"><span data-stu-id="4246e-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="4246e-121">A: setarea "BitLocker enabled" din Politica de conformitate Intune utilizeaza clientul Windows Device Atestation Health (DHA).</span><span class="sxs-lookup"><span data-stu-id="4246e-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="4246e-122">Acest client măsoară numai starea dispozitivului la Boot Time.</span><span class="sxs-lookup"><span data-stu-id="4246e-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="4246e-123">Deci, dacă un dispozitiv nu a fost repornit deoarece criptare BitLocker s-a finalizat, serviciul de client DHA nu va raporta BitLocker ca fiind activ.</span><span class="sxs-lookup"><span data-stu-id="4246e-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 