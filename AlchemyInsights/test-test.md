---
title: Termeni lipsă din SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053525"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="78256-102">Activarea criptare BitLocker cu Intune</span><span class="sxs-lookup"><span data-stu-id="78256-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="78256-103">Politica de protecție Intune Endpoint poate fi utilizată pentru a configura setările de criptare Boitlocker pentru dispozitivele Windows, așa este descris în: Windows10 (și versiunile ulterioare) pentru a proteja dispozitivele utilizând Intune</span><span class="sxs-lookup"><span data-stu-id="78256-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="78256-104">Trebuie să știți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată a BitLocker care este declanșată fără aplicarea politicii MDM.</span><span class="sxs-lookup"><span data-stu-id="78256-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="78256-105">Acest lucru poate afecta aplicarea politicii dacă nu sunt configurate setări implicite.</span><span class="sxs-lookup"><span data-stu-id="78256-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="78256-106">Consultați întrebări frecvente pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="78256-106">See FAQ for more detail.</span></span>


<span data-ttu-id="78256-107">Întrebări  frecvente: ce ediții de criptare dispozitiv de suport Windows utilizând politica de protecție Endpoint?</span><span class="sxs-lookup"><span data-stu-id="78256-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="78256-108"> A: setările în Intune Endpoint Protection politica sunt implementate utilizând CSP-ul BitLocker.</span><span class="sxs-lookup"><span data-stu-id="78256-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="78256-109">Nu toate edițiile și nici compilările de Windows acceptă CSP-ul BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="78256-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="78256-110">În acest moment Windows Editions: Enterprise; Educație, mobile, Mobile Enterprise și Professional (de la Build 1809 începând) sunt suportate.</span><span class="sxs-lookup"><span data-stu-id="78256-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="78256-111">Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite ale sistemului de operare pentru metoda de criptare și puterea cifrului (XTS-AES-128) va aplica o politică cu diferite setări declanșează automat re-criptarea unității cu noile setări?</span><span class="sxs-lookup"><span data-stu-id="78256-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="78256-112">A: nu.</span><span class="sxs-lookup"><span data-stu-id="78256-112">A: No.</span></span> <span data-ttu-id="78256-113">Pentru a aplica noile setări de cifrare, unitatea trebuie decriptată mai întâi.</span><span class="sxs-lookup"><span data-stu-id="78256-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="78256-114">Notă pentru dispozitivele care se înscriu cu autopilot criptarea automată care ar apărea în timpul OOBE nu este declanșată până când politica Intune este evaluată care permite setările de politică bazate pentru a fi utilizate în locul implicite de sistem de operare</span><span class="sxs-lookup"><span data-stu-id="78256-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="78256-115">Q dacă un dispozitiv este criptat ca urmare a aplicării politicii Intune va fi decriptat atunci când această politică este eliminată?</span><span class="sxs-lookup"><span data-stu-id="78256-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="78256-116">A: eliminarea politicii legate de criptare nu duce la decriptarea unităților care au fost configurate.</span><span class="sxs-lookup"><span data-stu-id="78256-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="78256-117">Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are "BitLocker enabled", dar este?</span><span class="sxs-lookup"><span data-stu-id="78256-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="78256-118">A: setarea "BitLocker enabled" în Politica de conformitate Intune utilizeaza clientul Windows Device sănătate Atestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="78256-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="78256-119">Acest client măsoară numai starea dispozitivului la Boot Time.</span><span class="sxs-lookup"><span data-stu-id="78256-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="78256-120">Deci, dacă un dispozitiv nu a fost repornit deoarece criptare BitLocker s-a finalizat serviciul de client DHA nu va raporta BitLocker ca fiind activ.</span><span class="sxs-lookup"><span data-stu-id="78256-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>