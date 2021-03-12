---
title: Criptarea automată a mesajelor de e-mail Office 365 trimise anumitor domenii
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749303"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="6a2f0-102">Criptarea automată a mesajelor de e-mail Office 365 trimise anumitor domenii</span><span class="sxs-lookup"><span data-stu-id="6a2f0-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="6a2f0-103">Din [Centrul de administrare Exchange](https://outlook.office365.com/ecp/), alegeți **regulile de > flux de corespondență**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="6a2f0-104">Faceți clic pe pictograma **nouă (+)** , apoi faceți clic pe **se aplică criptarea mesajelor Office 365 și protecția drepturilor la mesaje**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="6a2f0-105">În **nume**, introduceți un nume pentru regulă, cum ar fi *Criptarea mesajelor trimise către contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="6a2f0-106">În **se aplică această regulă dacă**, alegeți **domeniul > destinatarului**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="6a2f0-107">Introduceți numele domeniului, cum ar fi **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="6a2f0-108">Faceți clic pe pictograma **Add (+)** , apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="6a2f0-109">Lângă câmpul **fă următorul** , faceți clic pe **Selectare**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="6a2f0-110">În meniul vertical **șablon RMS** , selectați **criptare**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="6a2f0-111">(Dacă nu vedeți această opțiune, înseamnă că planul nu include criptarea automată.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="6a2f0-112">Dar îl puteți adăuga!)</span><span class="sxs-lookup"><span data-stu-id="6a2f0-112">But you can add it!)</span></span>
9. <span data-ttu-id="6a2f0-113">Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi lăsate cu setarea implicită pentru simplitate).</span><span class="sxs-lookup"><span data-stu-id="6a2f0-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="6a2f0-114">Faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6a2f0-115">Puteți oricând să reveniți și să editați această regulă mai târziu.</span><span class="sxs-lookup"><span data-stu-id="6a2f0-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="6a2f0-116">Pentru mai multe informații despre crearea regulilor de criptare, consultați [definirea regulilor de flux de corespondență pentru a cripta mesajele de e-mail în Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="6a2f0-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>