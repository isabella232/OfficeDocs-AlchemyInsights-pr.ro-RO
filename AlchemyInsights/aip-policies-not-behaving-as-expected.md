---
title: 'AIP: Politicile nu se comportă așa cum vă așteptați'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821639"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="d542b-102">AIP: Politicile nu se comportă așa cum vă așteptați</span><span class="sxs-lookup"><span data-stu-id="d542b-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="d542b-103">Azure Information Protection: Politicile nu au un comportament așa cum vă așteptați, consultați următoarele pentru instrucțiuni recomandate pentru diverse probleme de politică:</span><span class="sxs-lookup"><span data-stu-id="d542b-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="d542b-104">Dacă aveți probleme cu marcajele vizuale, revizuiți [Atunci când se aplică marcaje vizuale.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="d542b-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="d542b-105">Dacă aveți probleme cu etichetarea automată, revizuiți Cum se configurează condițiile pentru clasificarea automată și recomandată pentru [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și Ce tipuri de informații sensibile [caută.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d542b-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="d542b-106">Dacă aveți probleme cu protecția Native/Pfile, revizuiți [configurația FILE API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="d542b-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="d542b-107">Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: Cum se configurează politica [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)pentru utilizatori specifici utilizând politici de domeniu.</span><span class="sxs-lookup"><span data-stu-id="d542b-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="d542b-108">Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, verificați dacă DRMEncryptProperty nu este definit după cum este descris aici: Setări de [registry IRM](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)pentru securitate.</span><span class="sxs-lookup"><span data-stu-id="d542b-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="d542b-109">Dacă încă aveți probleme, colectați jurnale ale clientului Azure Information Protection și atașați jurnalele exportate la acest tichet.</span><span class="sxs-lookup"><span data-stu-id="d542b-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="d542b-110">Deschideți un document Office sau creați un mesaj de e-mail nou în Outlook.</span><span class="sxs-lookup"><span data-stu-id="d542b-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="d542b-111">Faceți clic pe Ajutor și feedback **pentru**  >  **protejare/sensibilitate.**</span><span class="sxs-lookup"><span data-stu-id="d542b-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="d542b-112">Faceți **clic pe Export jurnale.**</span><span class="sxs-lookup"><span data-stu-id="d542b-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="d542b-113">Salvați jurnalele la alegerea locației și atașați-le la această solicitare de serviciu.</span><span class="sxs-lookup"><span data-stu-id="d542b-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="d542b-114">Resurse suplimentare:</span><span class="sxs-lookup"><span data-stu-id="d542b-114">Additional resources:</span></span>

- [<span data-ttu-id="d542b-115">Cum se configurează o etichetă pentru marcajele vizuale pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d542b-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="d542b-116">Revizuiți documentația Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d542b-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d542b-117">Utilizați etichete de sensibilitate în aplicațiile Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d542b-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

