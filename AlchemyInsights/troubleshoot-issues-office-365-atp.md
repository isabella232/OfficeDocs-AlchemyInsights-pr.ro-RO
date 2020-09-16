---
title: Depanarea problemelor cu Office 365 Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758077"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c8faa-102">Depanarea problemelor cu Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="c8faa-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c8faa-103">**Observați întârzieri cu livrarea mesajelor de e-mail**?</span><span class="sxs-lookup"><span data-stu-id="c8faa-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="c8faa-104">Încercați să utilizați opțiunea de livrare dinamică pentru politicile de atașări sigure pentru ATP.</span><span class="sxs-lookup"><span data-stu-id="c8faa-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c8faa-105">Acest lucru va evita întârzierile livrării mesajelor de e-mail în timp ce protejează destinatarii din fișiere rău intenționate.</span><span class="sxs-lookup"><span data-stu-id="c8faa-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c8faa-106">**Doriți să raportați pozitive false sau negative false**?</span><span class="sxs-lookup"><span data-stu-id="c8faa-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="c8faa-107">Utilizați acest link pentru a trimite fișierul pentru analiză: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c8faa-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c8faa-108">**Știați că puteți permite protecția linkurilor de siguranță ATP pentru mesajele de e-mail trimise între persoanele din organizația dvs**.?</span><span class="sxs-lookup"><span data-stu-id="c8faa-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="c8faa-109">Urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="c8faa-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c8faa-110">Accesați https://protection.office.com și conectați-vă.</span><span class="sxs-lookup"><span data-stu-id="c8faa-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c8faa-111">Accesați **Threat management**  >  **Policy**  >  **linkuri sigure**pentru Politica de gestionare a amenințărilor.</span><span class="sxs-lookup"><span data-stu-id="c8faa-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="c8faa-112">Sub **politici care se aplică pentru anumiți destinatari**, editați (sau adăugați) o politică.</span><span class="sxs-lookup"><span data-stu-id="c8faa-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c8faa-113">Selectați **se aplică Linkuri sigure la mesajele trimise în cadrul Organizației**.</span><span class="sxs-lookup"><span data-stu-id="c8faa-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="c8faa-114">Salvați politica și permiteți aproximativ 30 de minute pentru ca modificările să funcționeze în centrul de date.</span><span class="sxs-lookup"><span data-stu-id="c8faa-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c8faa-115">Pentru a obține mai mult ajutor pentru ATP, consultați [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="c8faa-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>