---
title: 'AIP: politicile nu se poartă așa cum vă așteptați'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663201"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="d9c31-102">AIP: politicile nu se poartă așa cum vă așteptați</span><span class="sxs-lookup"><span data-stu-id="d9c31-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="d9c31-103">Azure Information Protection: politicile care nu se poartă așa cum vă așteptați, consultați următoarele instrucțiuni pentru recomandările recomandate pentru diverse probleme de politică:</span><span class="sxs-lookup"><span data-stu-id="d9c31-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="d9c31-104">Dacă întâmpinați probleme cu marcajele vizuale, vă rugăm să revizuiți [atunci când se aplică marcaje vizuale](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="d9c31-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="d9c31-105">Dacă întâmpinați probleme cu etichetarea automată, consultați [cum să configurați condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și [ce caută tipurile sensibile de informații](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="d9c31-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="d9c31-106">Dacă întâmpinați probleme cu protecția nativ/Pfile, examinați [configurația API a fișierelor](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="d9c31-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="d9c31-107">Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: [cum se configurează Politica de protecție a informațiilor Azure pentru anumiți utilizatori, utilizând politicile de domeniu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="d9c31-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="d9c31-108">Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, Verificați dacă DRMEncryptProperty nu este definit așa cum este descris aici: [setările de registry IRM pentru securitate](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="d9c31-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="d9c31-109">Dacă întâmpinați în continuare probleme, vă rugăm să colectați jurnalele clienților Azure Information Protection și să atașați jurnalele exportate la acest bilet.</span><span class="sxs-lookup"><span data-stu-id="d9c31-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="d9c31-110">Deschideți un document Office sau creați un mesaj de e-mail nou în Outlook.</span><span class="sxs-lookup"><span data-stu-id="d9c31-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="d9c31-111">Faceți clic pe **Protejare/sensibilitate**  >  **Ajutor și feedback**.</span><span class="sxs-lookup"><span data-stu-id="d9c31-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="d9c31-112">Faceți clic pe **Export jurnale**.</span><span class="sxs-lookup"><span data-stu-id="d9c31-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="d9c31-113">Salvați jurnalele la alegerea locației și atașați-le la această solicitare de serviciu.</span><span class="sxs-lookup"><span data-stu-id="d9c31-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="d9c31-114">Resurse suplimentare:</span><span class="sxs-lookup"><span data-stu-id="d9c31-114">Additional resources:</span></span>

- [<span data-ttu-id="d9c31-115">Cum se configurează o etichetă pentru marcaje vizuale pentru Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d9c31-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="d9c31-116">Revizuirea documentației Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d9c31-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d9c31-117">Utilizarea etichetelor de sensibilitate în aplicațiile Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d9c31-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

