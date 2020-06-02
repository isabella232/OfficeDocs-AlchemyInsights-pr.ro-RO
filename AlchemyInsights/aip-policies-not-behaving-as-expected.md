---
title: 'AIP: Politicile nu se comportă conform așteptărilor'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493415"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="f70b7-102">AIP: Politicile nu se comportă conform așteptărilor</span><span class="sxs-lookup"><span data-stu-id="f70b7-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="f70b7-103">Azure informații protecția: Politicile nu se comportă conform așteptărilor, consultați următoarele pentru liniile directoare recomandate pentru diverse probleme de politică:</span><span class="sxs-lookup"><span data-stu-id="f70b7-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="f70b7-104">Dacă aveți probleme cu marcajele vizuale, vă rugăm să examinați [Când se aplică marcajele vizuale](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="f70b7-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="f70b7-105">Dacă aveți probleme cu etichetarea automată, consultați [Cum se configurează condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="f70b7-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="f70b7-106">Dacă aveți probleme cu protecția native / Pfile, vă rugăm să revizuiți [configurația File API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="f70b7-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="f70b7-107">Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: [Cum se configurează politica azure protecția informațiilor pentru anumiți utilizatori utilizând politici ledomeniu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="f70b7-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="f70b7-108">Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, verificați dacă DRMEncryptProperty nu este definit așa este descris aici: [Setările de registry IRM pentru securitate](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="f70b7-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="f70b7-109">Dacă vă confruntați în continuare probleme, vă rugăm să colecteze Jurnalele de client Azure Information Protection și atașați jurnalele exportate la acest bilet.</span><span class="sxs-lookup"><span data-stu-id="f70b7-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="f70b7-110">Deschideți un document Office sau creați un e-mail nou în Outlook.</span><span class="sxs-lookup"><span data-stu-id="f70b7-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="f70b7-111">Faceți clic pe Ajutor și feedback **pentru protecție/sensibilitate**  >  **Help and feedback**.</span><span class="sxs-lookup"><span data-stu-id="f70b7-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="f70b7-112">Faceți clic pe **Export jurnale**.</span><span class="sxs-lookup"><span data-stu-id="f70b7-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="f70b7-113">Salvați jurnalele la alegerea locației și atașați-le la această solicitare de serviciu.</span><span class="sxs-lookup"><span data-stu-id="f70b7-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="f70b7-114">Resurse suplimentare:</span><span class="sxs-lookup"><span data-stu-id="f70b7-114">Additional resources:</span></span>

- [<span data-ttu-id="f70b7-115">se configurează o etichetă pentru marcaje vizuale pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f70b7-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="f70b7-116">Examinați documentația Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f70b7-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f70b7-117">Utilizarea etichetelor de sensibilitate în aplicațiile Office</span><span class="sxs-lookup"><span data-stu-id="f70b7-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

