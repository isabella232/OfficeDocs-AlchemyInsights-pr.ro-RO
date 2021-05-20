---
title: Depanarea Microsoft Defender pentru Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545280"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="f0274-102">Depanarea Microsoft Defender pentru Office 365</span><span class="sxs-lookup"><span data-stu-id="f0274-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="f0274-103">**Observați întârzieri în livrarea mesajelor?**</span><span class="sxs-lookup"><span data-stu-id="f0274-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="f0274-104">Utilizați opțiunea [Livrare dinamică](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) din politica Microsoft Defender pentru Office 365 Seif atașări.</span><span class="sxs-lookup"><span data-stu-id="f0274-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="f0274-105">Acest lucru vă va ajuta să evitați întârzierile mesajelor în timp ce protejați destinatarii de fișiere rău intenționate.</span><span class="sxs-lookup"><span data-stu-id="f0274-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="f0274-106">**Doriți să raportați rezultatele fals pozitive sau fals negative la Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="f0274-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="f0274-107">Utilizați [Remitere Explorer](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="f0274-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="f0274-108">-\*\* Știți că puteți activa protecția linkurilor Seif pentru mesajele de e-mail interne trimise între destinatarii din cadrul organizației dvs.?\*\* Urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="f0274-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="f0274-109">Accesați și [https://protection.office.com](https://protection.office.com) conectați-vă cu un cont de administrator global sau de administrator de securitate.</span><span class="sxs-lookup"><span data-stu-id="f0274-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="f0274-110">În panoul de navigare din stânga, sub **Gestionarea amenințărilor,** **alegeți Linkuri** \> **Seif politică.**</span><span class="sxs-lookup"><span data-stu-id="f0274-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="f0274-111">În **Politicile care se aplică la întreaga secțiune a organizației,** selectați politica și faceți clic pe **Editare**.</span><span class="sxs-lookup"><span data-stu-id="f0274-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="f0274-112">Sub **Setări**, activați **Se aplică linkuri sigure la mesajele trimise în cadrul organizației**.</span><span class="sxs-lookup"><span data-stu-id="f0274-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
