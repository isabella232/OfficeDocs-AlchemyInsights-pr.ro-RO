---
title: Criptarea automată a anumitor mesaje de e-mail Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526739"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="5c988-102">Criptarea automată a anumitor mesaje de e-mail Office 365</span><span class="sxs-lookup"><span data-stu-id="5c988-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="5c988-103">Puteți cripta automat mesajele pe care utilizatorii le trimit anumitor persoane sau organizații externe.</span><span class="sxs-lookup"><span data-stu-id="5c988-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="5c988-104">Pentru a face acest lucru, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="5c988-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="5c988-105">Din [Centrul de administrare Exchange](https://outlook.office365.com/ecp/), alegeți **regulile de > flux de corespondență**.</span><span class="sxs-lookup"><span data-stu-id="5c988-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="5c988-106">Faceți clic pe pictograma **nouă (+)** , apoi faceți clic pe **se aplică criptarea mesajelor Office 365 și protecția drepturilor la mesaje**.</span><span class="sxs-lookup"><span data-stu-id="5c988-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="5c988-107">În **nume**, introduceți un nume pentru regulă, cum ar fi *Criptarea mesajelor trimise către DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="5c988-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="5c988-108">În **se aplică această regulă dacă**, alegeți **> destinatar este această persoană**.</span><span class="sxs-lookup"><span data-stu-id="5c988-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="5c988-109">În fereastra **Selectare membri** , selectați numele persoanei la care doriți să se aplice regula de criptare, apoi faceți clic pe **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="5c988-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="5c988-110">Când ați terminat de adăugat utilizatori, faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="5c988-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="5c988-111">Lângă câmpul **fă următorul** , faceți clic pe **Selectare**.</span><span class="sxs-lookup"><span data-stu-id="5c988-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="5c988-112">În meniul vertical **șablon RMS** , selectați **criptare**, apoi faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="5c988-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="5c988-113">(Dacă nu vedeți această opțiune, înseamnă că planul nu include criptarea automată.</span><span class="sxs-lookup"><span data-stu-id="5c988-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="5c988-114">Dar îl puteți adăuga!)</span><span class="sxs-lookup"><span data-stu-id="5c988-114">But you can add it!)</span></span>
9. <span data-ttu-id="5c988-115">Alegeți orice selecție opțională (dintr-o listă de selecții opționale pe care le puteți face în acest moment, dintre care multe pot fi lăsate cu setarea implicită pentru simplitate).</span><span class="sxs-lookup"><span data-stu-id="5c988-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="5c988-116">Faceți clic pe **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="5c988-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5c988-117">Puteți oricând să reveniți și să editați această regulă mai târziu.</span><span class="sxs-lookup"><span data-stu-id="5c988-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="5c988-118">Pentru mai multe informații despre crearea regulilor de criptare, consultați [definirea regulilor de flux de corespondență pentru a cripta mesajele de e-mail în Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="5c988-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

