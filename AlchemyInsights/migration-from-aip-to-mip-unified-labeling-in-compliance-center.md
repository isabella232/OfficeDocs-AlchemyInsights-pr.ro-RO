---
title: Migrarea de la AIP la PMI/etichetarea unificată în centrul de conformitate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674338"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="8553f-102">Migrarea de la AIP la PMI/etichetarea unificată în centrul de conformitate</span><span class="sxs-lookup"><span data-stu-id="8553f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="8553f-103">Pentru a migra de la etichetele AIP la etichetarea unificată în centrul de securitate și conformitate, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="8553f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="8553f-104">**Activarea protecției din portalul Azure**</span><span class="sxs-lookup"><span data-stu-id="8553f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="8553f-105">Dacă nu ați făcut deja acest lucru, deschideți o fereastră nouă de browser și [Conectați-vă la portalul Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="8553f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="8553f-106">Navigați la lama de **protecție a informațiilor Azure** .</span><span class="sxs-lookup"><span data-stu-id="8553f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="8553f-107">De exemplu, în meniul hub, faceți clic pe **toate serviciile** și începeți să tastați **informații** în caseta de filtrare.</span><span class="sxs-lookup"><span data-stu-id="8553f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="8553f-108">Selectați **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="8553f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="8553f-109">Dacă nu ați mai accesat lama Azure Information Protection înainte, consultați [pașii suplimentari](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pentru a adăuga această lamă la portal.</span><span class="sxs-lookup"><span data-stu-id="8553f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="8553f-110">Pentru a deschide lama Azure Information Protection, trebuie să aveți fie un [plan Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) , fie un plan 365 Office care include managementul drepturilor.</span><span class="sxs-lookup"><span data-stu-id="8553f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="8553f-111">Dacă aveți unul dintre aceste abonamente, dar vedeți un mesaj că nu se poate găsi un abonament valid, [contactați asistența Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) sau utilizați canalele de asistență standard.</span><span class="sxs-lookup"><span data-stu-id="8553f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="8553f-112">Găsiți opțiunile de meniu **gestionare** și selectați **activare protecție**.</span><span class="sxs-lookup"><span data-stu-id="8553f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="8553f-113">Faceți clic pe **Activare**, apoi confirmați acțiunea.</span><span class="sxs-lookup"><span data-stu-id="8553f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="8553f-114">Când Activarea este finalizată, bara de informații afișează **Activarea terminată cu succes**.</span><span class="sxs-lookup"><span data-stu-id="8553f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="8553f-115">**Migrarea etichetelor de protecție Azure Information la Office 365 Security & Conformity Center**</span><span class="sxs-lookup"><span data-stu-id="8553f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="8553f-116">Asigurați-vă că sunteți conectat ca utilizator cu permisiunea de administrator global.</span><span class="sxs-lookup"><span data-stu-id="8553f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="8553f-117">Navigați la lama de **protecție a informațiilor Azure** .</span><span class="sxs-lookup"><span data-stu-id="8553f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="8553f-118">Din opțiunea **gestionare** meniu, selectați **etichetare unificată**.</span><span class="sxs-lookup"><span data-stu-id="8553f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="8553f-119">În secțiunea **Azure Information Protection-lamă de etichetare unificată** , faceți clic pe **Activare** și urmați instrucțiunile online.</span><span class="sxs-lookup"><span data-stu-id="8553f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="8553f-120">**Notă**: Verificați dacă aveți permisiunile corespunzătoare înainte de a activa migrarea în centrul de securitate & de conformitate.</span><span class="sxs-lookup"><span data-stu-id="8553f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="8553f-121">Consultați aceste articole pentru mai multe informații:</span><span class="sxs-lookup"><span data-stu-id="8553f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="8553f-122">Trebuie să fiți administrator global pentru a configura Azure Information Protection sau pot să delege altor administratori?</span><span class="sxs-lookup"><span data-stu-id="8553f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="8553f-123">Informații importante despre rolurile administrative după migrarea la centrul de conformitate & pentru securitate.</span><span class="sxs-lookup"><span data-stu-id="8553f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="8553f-124">Pentru mai multe informații despre AIP la migrarea unificată a etichetelor către centrul de securitate și conformitate, consultați [migrarea etichetelor](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="8553f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
