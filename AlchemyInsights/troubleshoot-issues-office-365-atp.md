---
title: Depanarea problemelor cu Microsoft Defender pentru Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801419"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="7cdea-102">Depanarea problemelor cu Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="7cdea-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="7cdea-103">**Observați întârzieri cu livrarea mesajelor de e-mail** ?</span><span class="sxs-lookup"><span data-stu-id="7cdea-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="7cdea-104">Încercați să utilizați opțiunea de livrare dinamică pentru politicile de atașări sigure pentru ATP.</span><span class="sxs-lookup"><span data-stu-id="7cdea-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="7cdea-105">Acest lucru va evita întârzierile livrării mesajelor de e-mail în timp ce protejează destinatarii din fișiere rău intenționate.</span><span class="sxs-lookup"><span data-stu-id="7cdea-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="7cdea-106">**Doriți să raportați pozitive false sau negative false** ?</span><span class="sxs-lookup"><span data-stu-id="7cdea-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="7cdea-107">Utilizați acest link pentru a trimite fișierul pentru analiză: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="7cdea-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="7cdea-108">**Știați că puteți permite protecția linkurilor de siguranță ATP pentru mesajele de e-mail trimise între persoanele din organizația dvs** .?</span><span class="sxs-lookup"><span data-stu-id="7cdea-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="7cdea-109">Urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="7cdea-109">Follow these steps:</span></span>
    1. <span data-ttu-id="7cdea-110">Accesați https://protection.office.com și conectați-vă.</span><span class="sxs-lookup"><span data-stu-id="7cdea-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="7cdea-111">Accesați **Threat management**  >  **Policy**  >  **linkuri sigure** pentru Politica de gestionare a amenințărilor.</span><span class="sxs-lookup"><span data-stu-id="7cdea-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="7cdea-112">Sub **politici care se aplică pentru anumiți destinatari** , editați (sau adăugați) o politică.</span><span class="sxs-lookup"><span data-stu-id="7cdea-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="7cdea-113">Selectați **se aplică Linkuri sigure la mesajele trimise în cadrul Organizației** .</span><span class="sxs-lookup"><span data-stu-id="7cdea-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="7cdea-114">Salvați politica și permiteți aproximativ 30 de minute pentru ca modificările să funcționeze în centrul de date.</span><span class="sxs-lookup"><span data-stu-id="7cdea-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="7cdea-115">Pentru a obține mai mult ajutor pentru ATP, consultați [Microsoft Defender pentru Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="7cdea-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>