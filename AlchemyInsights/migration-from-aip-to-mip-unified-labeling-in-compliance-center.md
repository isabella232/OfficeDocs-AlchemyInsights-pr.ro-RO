---
title: Migrarea de la AIP la eticheta MIP/Unificată în Centrul de conformitate
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825383"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="1c273-102">Migrarea de la AIP la eticheta MIP/Unificată în Centrul de conformitate</span><span class="sxs-lookup"><span data-stu-id="1c273-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="1c273-103">Pentru a migra de la etichete AIP la Etichetare unificată în Centrul de securitate și conformitate, efectuați următoarele:</span><span class="sxs-lookup"><span data-stu-id="1c273-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="1c273-104">**Activarea protecției din portalul Azure**</span><span class="sxs-lookup"><span data-stu-id="1c273-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="1c273-105">Dacă nu ați făcut deja acest lucru, deschideți o fereastră nouă de browser [și conectați-vă la portalul Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="1c273-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="1c273-106">Navigați la **blade Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="1c273-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="1c273-107">De exemplu, în meniul hub, faceți clic **pe Toate serviciile** și începeți să **tastați** Informații în caseta Filtrare.</span><span class="sxs-lookup"><span data-stu-id="1c273-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="1c273-108">Selectați **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="1c273-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="1c273-109">Dacă nu ați accesat înainte sistemul blade Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection, consultați pașii suplimentari pentru adăugarea acestui blade în portal.</span><span class="sxs-lookup"><span data-stu-id="1c273-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="1c273-110">Pentru a deschide Azure Information Protection blade, trebuie să aveți un [plan Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) sau un plan Office 365 care include Rights Management.</span><span class="sxs-lookup"><span data-stu-id="1c273-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="1c273-111">Dacă aveți unul dintre aceste abonamente, dar vedeți un mesaj care spune că nu poate fi găsit un abonament valid, [contactați](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) Asistența Microsoft sau utilizați canalele de asistență standard.</span><span class="sxs-lookup"><span data-stu-id="1c273-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="1c273-112">Găsiți **opțiunile** din meniul Gestionare și selectați **Activare protecție.**</span><span class="sxs-lookup"><span data-stu-id="1c273-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="1c273-113">Faceți **clic** pe Activare , apoi confirmați acțiunea.</span><span class="sxs-lookup"><span data-stu-id="1c273-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="1c273-114">Atunci când activarea s-a terminat, bara de informații afișează **Activarea s-a finalizat cu succes.**</span><span class="sxs-lookup"><span data-stu-id="1c273-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="1c273-115">**Migrarea etichetelor Azure Information Protection la Centrul de securitate & Office 365**</span><span class="sxs-lookup"><span data-stu-id="1c273-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="1c273-116">Asigurați-vă că sunteți conectat ca utilizator cu permisiunea Administrator global.</span><span class="sxs-lookup"><span data-stu-id="1c273-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="1c273-117">Navigați la **blade Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="1c273-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="1c273-118">Din opțiunea **de** meniu Gestionare, **selectați Etichetare unificată**.</span><span class="sxs-lookup"><span data-stu-id="1c273-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="1c273-119">Pe **Azure Information Protection - etichetare unificată** blade, faceți clic pe **Activare și** urmați instrucțiunile online.</span><span class="sxs-lookup"><span data-stu-id="1c273-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="1c273-120">**Notă:** Verificați dacă aveți permisiunile corespunzătoare înainte de a activa Migrarea Centrului & de conformitate.</span><span class="sxs-lookup"><span data-stu-id="1c273-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="1c273-121">Consultați aceste articole pentru mai multe informații:</span><span class="sxs-lookup"><span data-stu-id="1c273-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="1c273-122">Trebuie să fiți administrator global pentru a configura Azure Information Protection sau pot delega altor administratori?</span><span class="sxs-lookup"><span data-stu-id="1c273-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="1c273-123">Informații importante despre rolurile administrative după migrarea la Centrul de & conformitate.</span><span class="sxs-lookup"><span data-stu-id="1c273-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="1c273-124">Pentru mai multe informații despre AIP la Centrul unificat de etichetare a migrării la Centrul de securitate și conformitate, consultați [Migrarea etichetelor.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="1c273-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
