---
title: Criptarea automată a anumitor mesaje de e-mail din Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749459"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="b4461-102">Criptarea automată a anumitor mesaje de e-mail din Office 365</span><span class="sxs-lookup"><span data-stu-id="b4461-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="b4461-103">Din [Centrul de administrare Exchange](https://outlook.office365.com/ecp/), alegeți **regulile de > flux de corespondență**.</span><span class="sxs-lookup"><span data-stu-id="b4461-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="b4461-104">Faceți clic pe pictograma **nouă (+)** , apoi faceți clic pe **se aplică criptarea mesajelor Office 365 și protecția drepturilor la mesaje**.</span><span class="sxs-lookup"><span data-stu-id="b4461-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="b4461-105">În **nume**, introduceți un nume pentru regulă, cum ar fi *Criptarea tuturor mesajelor*.</span><span class="sxs-lookup"><span data-stu-id="b4461-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="b4461-106">În **se aplică această regulă dacă**, alegeți **[se aplică la toate mesajele]**.</span><span class="sxs-lookup"><span data-stu-id="b4461-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="b4461-107">Lângă câmpul **fă următorul** , faceți clic pe **Selectare**.</span><span class="sxs-lookup"><span data-stu-id="b4461-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="b4461-108">În meniul vertical **șablon RMS** , selectați **criptare**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="b4461-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="b4461-109">(Dacă nu vedeți această opțiune, înseamnă că planul nu include criptarea automată.</span><span class="sxs-lookup"><span data-stu-id="b4461-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="b4461-110">Dar îl puteți adăuga!)</span><span class="sxs-lookup"><span data-stu-id="b4461-110">But you can add it!)</span></span>
7. <span data-ttu-id="b4461-111">Bifați caseta de selectare **auditare regulă cu nivel de severitate** , apoi selectați nivelul dorit.</span><span class="sxs-lookup"><span data-stu-id="b4461-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="b4461-112">Dacă firma dumneavoastră are obligații contractuale de a trimite toate mesajele de e-mail criptate, vă recomandăm să setați nivelul la **maxim**.</span><span class="sxs-lookup"><span data-stu-id="b4461-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="b4461-113">Sub **alegere model pentru această regulă**, faceți clic pe **aplicare**.</span><span class="sxs-lookup"><span data-stu-id="b4461-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="b4461-114">Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi lăsate cu setarea implicită pentru simplitate).</span><span class="sxs-lookup"><span data-stu-id="b4461-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="b4461-115">Faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="b4461-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b4461-116">Puteți oricând să reveniți și să editați această regulă mai târziu.</span><span class="sxs-lookup"><span data-stu-id="b4461-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="b4461-117">Pentru mai multe informații despre crearea regulilor de criptare, consultați [definirea regulilor de flux de corespondență pentru a cripta mesajele de e-mail în Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="b4461-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

