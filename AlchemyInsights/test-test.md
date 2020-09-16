---
title: Condiții lipsă din depozitul de termeni SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750463"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="4f8f7-102">Activarea criptării BitLocker cu Intune</span><span class="sxs-lookup"><span data-stu-id="4f8f7-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="4f8f7-103">Politica de protecție a Endpoint-ului Intune poate fi utilizată pentru a configura setările de criptare Boitlocker pentru dispozitivele Windows, așa cum este descris în: Windows10 (și versiuni mai recente) pentru a proteja dispozitivele utilizând Intune</span><span class="sxs-lookup"><span data-stu-id="4f8f7-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="4f8f7-104">Trebuie să rețineți că multe dispozitive mai noi care rulează Windows 10 acceptă criptarea automată BitLocker care este declanșată fără aplicarea politicii MDM.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="4f8f7-105">Acest lucru poate avea un impact asupra aplicării politicii dacă sunt configurate setările non-implicite.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="4f8f7-106">Consultați întrebări frecvente pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-106">See FAQ for more detail.</span></span>


<span data-ttu-id="4f8f7-107">Întrebări frecvente   î: ce ediții de criptare a dispozitivelor de asistență Windows utilizând politica de protecție pentru Endpoint?</span><span class="sxs-lookup"><span data-stu-id="4f8f7-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="4f8f7-108"> A: Politica de protecție a Endpoint-ului setări din Intune este implementată utilizând CSP-ul BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="4f8f7-109">Nu toate edițiile și versiunile de Windows acceptă CSP-ul BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="4f8f7-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="4f8f7-110">În acest moment edițiile Windows: Enterprise; Sunt acceptate educația, telefonul mobil, întreprinderea mobilă și Professional (de la compilarea 1809 începând cu).</span><span class="sxs-lookup"><span data-stu-id="4f8f7-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="4f8f7-111">Î: dacă un dispozitiv este deja criptat cu BitLocker utilizând setările implicite de sistem de operare pentru metoda de criptare și puterea cifrului (XTS-AES-128) va aplica o politică cu setări diferite, declanșând automat recriptarea unității cu noile setări?</span><span class="sxs-lookup"><span data-stu-id="4f8f7-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="4f8f7-112">R: Nu.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-112">A: No.</span></span> <span data-ttu-id="4f8f7-113">Pentru a aplica noile setări de cifru, unitatea trebuie mai întâi decriptată.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="4f8f7-114">Notă pentru dispozitivele care se înscriu cu autopilot, criptarea automată care va apărea în timpul OOBE nu se declanșează până când politica Intune este evaluată, care permite ca setările bazate pe politică să fie utilizate în locul valorilor implicite pentru sistemul de operare</span><span class="sxs-lookup"><span data-stu-id="4f8f7-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="4f8f7-115">Î dacă un dispozitiv este criptat ca rezultat al aplicării politicii Intune, acesta va fi decriptat atunci când se elimină Politica?</span><span class="sxs-lookup"><span data-stu-id="4f8f7-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="4f8f7-116">A: eliminarea politicii legate de criptare nu determină decriptarea unităților care au fost configurate.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="4f8f7-117">Î: de ce politica de conformitate Intune arată că dispozitivul meu nu are "BitLocker activat", dar este?</span><span class="sxs-lookup"><span data-stu-id="4f8f7-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="4f8f7-118">A: setarea "BitLocker enabled" din Politica de conformitate Intune utilizeazã clientul de atestare a sanatatii dispozitivelor Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="4f8f7-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="4f8f7-119">Acest client măsoară doar starea dispozitivului în timpul încărcării.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="4f8f7-120">Așadar, dacă un dispozitiv nu a fost repornit, deoarece criptarea BitLocker a fost finalizată, serviciul client DHA nu va raporta BitLocker ca fiind activ.</span><span class="sxs-lookup"><span data-stu-id="4f8f7-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>