---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768829"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="23c62-102">Activarea criptării BitLocker cu Intune</span><span class="sxs-lookup"><span data-stu-id="23c62-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="23c62-103">Politica de protecție a Endpoint-ului Intune poate fi utilizată pentru a configura setările de criptare BitLocker pentru dispozitivele Windows.</span><span class="sxs-lookup"><span data-stu-id="23c62-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="23c62-104">Pentru mai multe informații, consultați [Setări Windows 10 (și versiuni mai recente) pentru a proteja dispozitivele utilizând Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="23c62-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="23c62-105">Trebuie să rețineți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată BitLocker, care este declanșată fără aplicarea politicii MDM.</span><span class="sxs-lookup"><span data-stu-id="23c62-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="23c62-106">Acest lucru poate avea un impact asupra aplicării politicii dacă sunt configurate setările non-implicite.</span><span class="sxs-lookup"><span data-stu-id="23c62-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="23c62-107">Consultați următoarele întrebări frecvente pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="23c62-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="23c62-108">Pentru informații despre depanarea problemelor cu BitLocker, consultați [Depanarea politicilor BitLocker în Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="23c62-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="23c62-109">**ÎNTREBĂRI FRECVENTE**</span><span class="sxs-lookup"><span data-stu-id="23c62-109">**FAQ**</span></span>

<span data-ttu-id="23c62-110">Î: ce ediții de Windows acceptă criptarea dispozitivelor folosind Politica de protecție a Endpoint?</span><span class="sxs-lookup"><span data-stu-id="23c62-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="23c62-111">A: Politica de protecție a Endpoint-ului setări din Intune este implementată utilizând CSP-ul [BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="23c62-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="23c62-112">Nu toate edițiile sau compilările Windows acceptă CSP-ul BitLocker.</span><span class="sxs-lookup"><span data-stu-id="23c62-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="23c62-113">Î: Cum poate fi activată BitLocker pe dispozitive fără a necesita interacțiune cu utilizatorul final?</span><span class="sxs-lookup"><span data-stu-id="23c62-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="23c62-114">A: atât timp cât sunt îndeplinite cerințele preliminare necesare, este posibil să activați BitLocker "Silent Encryption" prin Intune.</span><span class="sxs-lookup"><span data-stu-id="23c62-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="23c62-115">Vedeți detaliile cerințelor dispozitivului și exemple de politici pentru a activa criptarea silențioasă în următorul document: [activați în liniște criptarea BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="23c62-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="23c62-116">Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite de sistem de operare pentru metoda de criptare și tăria cifră (XTS-AES-128), va aplica o politică cu setări diferite care declanșează automat recriptarea unității cu noile setări?</span><span class="sxs-lookup"><span data-stu-id="23c62-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="23c62-117">R: Nu.</span><span class="sxs-lookup"><span data-stu-id="23c62-117">A: No.</span></span> <span data-ttu-id="23c62-118">Pentru a aplica noile setări de cifru, unitatea trebuie mai întâi decriptată.</span><span class="sxs-lookup"><span data-stu-id="23c62-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="23c62-119">**Notă:** Pentru dispozitivele care se înscriu cu autopilot, criptarea automată care va apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată, care permite utilizarea setărilor bazate pe politică în locul valorilor implicite pentru sistemul de operare.</span><span class="sxs-lookup"><span data-stu-id="23c62-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="23c62-120">Î: dacă un dispozitiv este criptat ca rezultat al aplicării politicii Intune, acesta va fi decriptat atunci când se elimină Politica?</span><span class="sxs-lookup"><span data-stu-id="23c62-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="23c62-121">A: eliminarea politicii legate de criptare nu determină decriptarea unităților care au fost configurate.</span><span class="sxs-lookup"><span data-stu-id="23c62-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="23c62-122">Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are BitLocker activat, chiar dacă este?</span><span class="sxs-lookup"><span data-stu-id="23c62-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="23c62-123">A: setarea "BitLocker enabled" din Politica de conformitate Intune utilizeazã clientul de atestare a sanatatii dispozitivelor Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="23c62-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="23c62-124">Acest client măsoară doar starea dispozitivului în timpul încărcării.</span><span class="sxs-lookup"><span data-stu-id="23c62-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="23c62-125">Așadar, dacă un dispozitiv nu a fost repornit de când s-a finalizat criptarea BitLocker, serviciul client DHA nu va raporta BitLocker ca fiind activ.</span><span class="sxs-lookup"><span data-stu-id="23c62-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 