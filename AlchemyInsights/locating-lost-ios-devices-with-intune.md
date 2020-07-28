---
title: Localizarea dispozitivelor iOS pierdute cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440426"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="7d897-102">Localizarea dispozitivelor iOS pierdute cu Intune</span><span class="sxs-lookup"><span data-stu-id="7d897-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="7d897-103">Activarea modului pierdut pe un dispozitiv iOS permite unui administrator să aibă un mesaj și un număr de telefon de contact afișat pe ecranul de blocare.</span><span class="sxs-lookup"><span data-stu-id="7d897-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="7d897-104">După activarea modului pierdut, administratorul poate utiliza acțiunea Localizare dispozitiv pentru a identifica locația fizică a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="7d897-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="7d897-105">Acțiunea Localizare dispozitiv din Intune funcționează cu dispozitive iOS pentru a afișa locația unui anumit dispozitiv pe o hartă.</span><span class="sxs-lookup"><span data-stu-id="7d897-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="7d897-106">Utilizarea acestei acțiuni necesită ca dispozitivul iOS să fie în:</span><span class="sxs-lookup"><span data-stu-id="7d897-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="7d897-107">Mod supravegheat</span><span class="sxs-lookup"><span data-stu-id="7d897-107">Supervised mode</span></span>
- <span data-ttu-id="7d897-108">Mod pierdut</span><span class="sxs-lookup"><span data-stu-id="7d897-108">Lost mode</span></span>

<span data-ttu-id="7d897-109">Pentru mai multe informații, consultați [Activarea modului pierdut pe dispozitivele iOS/iPadOS cu Intune](https://docs.microsoft.com/intune/device-lost-mode) și [Locate dispozitive iOS/iPadOS pierdute sau furate cu Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="7d897-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="7d897-110">**ÎNTREBĂRI FRECVENTE**</span><span class="sxs-lookup"><span data-stu-id="7d897-110">**FAQ**</span></span>

<span data-ttu-id="7d897-111">Î: Am emis o acțiune la distanță pentru a elimina datele companiei de pe un dispozitiv, iar acum este blocat într-o stare în așteptare.</span><span class="sxs-lookup"><span data-stu-id="7d897-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="7d897-112">R: Pentru ca o acțiune la distanță să se finalizeze cu succes, dispozitivul vizat trebuie să fie online și sănătos.</span><span class="sxs-lookup"><span data-stu-id="7d897-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="7d897-113">În următoarele situații, acțiunea la distanță rămâne într-o stare în așteptare timp de 30 de zile sau până când dispozitivul recunoaște comanda:</span><span class="sxs-lookup"><span data-stu-id="7d897-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="7d897-114">Când dispozitivul nu are conectivitate</span><span class="sxs-lookup"><span data-stu-id="7d897-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="7d897-115">Când dispozitivul își pierde starea de gestionare cu Intune</span><span class="sxs-lookup"><span data-stu-id="7d897-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="7d897-116">Dacă credeți că un dispozitiv nu se mai face check-in și că nu va putea elimina datele companiei, selectați Ștergere.</span><span class="sxs-lookup"><span data-stu-id="7d897-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="7d897-117">Ștergerea elimină înregistrarea dispozitivului, astfel încât să nu mai apară în lista de dispozitive Intune.</span><span class="sxs-lookup"><span data-stu-id="7d897-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="7d897-118">Dacă dispozitivul devine activ din nou, utilizatorul său va trebui să-l reînscrie.</span><span class="sxs-lookup"><span data-stu-id="7d897-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="7d897-119">Î: De ce anumite acțiuni la distanță nu sunt disponibile pentru mine?</span><span class="sxs-lookup"><span data-stu-id="7d897-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="7d897-120">R: Nu toate platformele acceptă toate acțiunile dispozitivelor la distanță.</span><span class="sxs-lookup"><span data-stu-id="7d897-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="7d897-121">Următoarele acțiuni la distanță sunt specifice platformei, astfel încât acestea sunt disponibile numai pentru platformele menționate.</span><span class="sxs-lookup"><span data-stu-id="7d897-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="7d897-122">Blocare activare bypass (numai iOS)</span><span class="sxs-lookup"><span data-stu-id="7d897-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="7d897-123">Pornire proaspătă (numai windows)</span><span class="sxs-lookup"><span data-stu-id="7d897-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="7d897-124">Mod pierdut (numai iOS)</span><span class="sxs-lookup"><span data-stu-id="7d897-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="7d897-125">Localizare dispozitiv (numai iOS)</span><span class="sxs-lookup"><span data-stu-id="7d897-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="7d897-126">Repornire (numai Windows)</span><span class="sxs-lookup"><span data-stu-id="7d897-126">Restart (Windows only)</span></span>

<span data-ttu-id="7d897-127">Pentru mai multe detalii despre fiecare acțiune, consultați [Acțiunile disponibile ale dispozitivului](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="7d897-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>