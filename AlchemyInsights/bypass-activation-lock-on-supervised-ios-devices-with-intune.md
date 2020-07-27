---
title: Bypass blocare de activare pe dispozitivele iOS supravegheate cu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424215"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="ea9c8-102">Bypass blocare de activare pe dispozitivele iOS supravegheate cu Intune</span><span class="sxs-lookup"><span data-stu-id="ea9c8-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="ea9c8-103">Capacitatea de a ocoli blocarea de activare pe dispozitivele iOS face mai ușor de recuperat din scenariul în care un utilizator permite blocarea de activare pe un dispozitiv corporativ, și apoi părăsește compania.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="ea9c8-104">Cerințele prealabile pentru a ocoli o blocare de activare includ:</span><span class="sxs-lookup"><span data-stu-id="ea9c8-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="ea9c8-105">Un dispozitiv este "supravegheat".</span><span class="sxs-lookup"><span data-stu-id="ea9c8-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="ea9c8-106">Blocarea activării este activată cu succes utilizând politica de restricționare a dispozitivului iOS în Intune.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="ea9c8-107">În plus, atunci când ocoliți o blocare de activare, ar trebui:</span><span class="sxs-lookup"><span data-stu-id="ea9c8-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="ea9c8-108">Posedă fizic dispozitivul fiind șters.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="ea9c8-109">Copiați codul înainte de a emite ștergerea.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="ea9c8-110">**Notă:** Codul de ștergere nu este sensibil la litere mari și mici, astfel încât caracterele "-" nu sunt necesare.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="ea9c8-111">Pentru detalii, consultați [Blocarea de activare bypass pe dispozitivele iOS supravegheate cu Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="ea9c8-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="ea9c8-112">**ÎNTREBĂRI FRECVENTE**</span><span class="sxs-lookup"><span data-stu-id="ea9c8-112">**FAQ**</span></span>

<span data-ttu-id="ea9c8-113">Î: **Am emis o acțiune la distanță pentru a elimina datele companiei de pe un dispozitiv, iar acum este blocat într-o stare în așteptare.**</span><span class="sxs-lookup"><span data-stu-id="ea9c8-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="ea9c8-114">R: Pentru ca o acțiune la distanță să se finalizeze cu succes, dispozitivul vizat trebuie să fie online și sănătos.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="ea9c8-115">În următoarele situații, acțiunea la distanță rămâne într-o stare în așteptare timp de 30 de zile sau până când dispozitivul recunoaște comanda atunci când dispozitivul:</span><span class="sxs-lookup"><span data-stu-id="ea9c8-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="ea9c8-116">Nu are conectivitate.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-116">Does not have connectivity.</span></span>
- <span data-ttu-id="ea9c8-117">Își pierde statutul de management cu Intune.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="ea9c8-118">Dacă credeți că un dispozitiv nu se mai face check-in și că nu va elimina datele companiei, selectați Ștergere.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="ea9c8-119">Ștergerea elimină înregistrarea dispozitivului, astfel încât să nu mai apară în lista de dispozitive Intune.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="ea9c8-120">Pentru ca dispozitivul să devină din nou activ, utilizatorul trebuie să reînscrie dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="ea9c8-121">Î: **De ce anumite acțiuni la distanță nu sunt disponibile pentru mine?**</span><span class="sxs-lookup"><span data-stu-id="ea9c8-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="ea9c8-122">R: Nu toate platformele acceptă toate acțiunile dispozitivelor la distanță.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="ea9c8-123">Următoarele acțiuni la distanță sunt specifice platformei.</span><span class="sxs-lookup"><span data-stu-id="ea9c8-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="ea9c8-124">Blocare activare bypass (numai iOS)</span><span class="sxs-lookup"><span data-stu-id="ea9c8-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="ea9c8-125">Pornire proaspătă (numai windows)</span><span class="sxs-lookup"><span data-stu-id="ea9c8-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="ea9c8-126">Mod pierdut (numai iOS)</span><span class="sxs-lookup"><span data-stu-id="ea9c8-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="ea9c8-127">Localizare dispozitiv (numai iOS)</span><span class="sxs-lookup"><span data-stu-id="ea9c8-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="ea9c8-128">Repornire (numai Windows)</span><span class="sxs-lookup"><span data-stu-id="ea9c8-128">Restart (Windows only)</span></span>

<span data-ttu-id="ea9c8-129">Pentru mai multe detalii despre fiecare acțiune, consultați [Acțiunile disponibile ale dispozitivului](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="ea9c8-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>