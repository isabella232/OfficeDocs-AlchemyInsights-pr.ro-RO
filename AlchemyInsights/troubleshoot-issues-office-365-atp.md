---
title: Depanarea problemelor cu Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766757"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="f0d5d-102">Depanarea problemelor cu Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="f0d5d-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="f0d5d-103">**Observați întârzieri cu livrarea mesajelor de e-mail?**</span><span class="sxs-lookup"><span data-stu-id="f0d5d-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="f0d5d-104">Încercați să utilizați opțiunea Livrare dinamică pentru politicile atp privind atașările sigure.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="f0d5d-105">Acest lucru va evita întârzierile de livrare a mesajelor de e-mail, protejând în același timp destinatarii de fișierele rău intenționate.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="f0d5d-106">**Raportați rezultate fals pozitive sau negative false?**</span><span class="sxs-lookup"><span data-stu-id="f0d5d-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="f0d5d-107">Utilizați acest link pentru a trimite fișierul pentru analiză:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="f0d5d-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="f0d5d-108">**Știați că puteți activa ATP Safe Link-uri de protecție pentru e-mail trimis între persoane din organizația dumneavoastră?**</span><span class="sxs-lookup"><span data-stu-id="f0d5d-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="f0d5d-109">Urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="f0d5d-109">Follow these steps:</span></span>
    1. <span data-ttu-id="f0d5d-110">Du-te la, https://protection.office.comși autentifică-te.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="f0d5d-111">Du-te la **Threat management** > **Policy** > **Safe Link-uri**.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="f0d5d-112">Sub **Politici care se aplică anumitor destinatari,** editați (sau adăugați) o politică.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="f0d5d-113">**Selectaþi Aplicaþii linkuri sigure la mesajele trimise în cadrul organizației**.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="f0d5d-114">Salvați politica și permiteți aproximativ 30 de minute ca modificările să își croiască drum prin centrul de date.</span><span class="sxs-lookup"><span data-stu-id="f0d5d-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="f0d5d-115">Pentru a obține mai mult ajutor pentru ATP, consultați [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="f0d5d-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>