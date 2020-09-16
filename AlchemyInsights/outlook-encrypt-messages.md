---
title: S/MIME în Outlook pe web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772310"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="2504a-102">Criptarea mesajelor de e-mail în Outlook</span><span class="sxs-lookup"><span data-stu-id="2504a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="2504a-103">Criptarea mesajelor Microsoft 365 este construită în Microsoft Azure Rights Management (Azure RMS), care face parte din Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="2504a-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="2504a-104">Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu trebuie să efectuați acțiuni pentru a activa sau a activa manual** serviciul de administrare a drepturilor.</span><span class="sxs-lookup"><span data-stu-id="2504a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="2504a-105">Pe baza feedbackului de la clienți, nu vom mai permite reguli de flux de corespondență Exchange pentru a cripta automat e-mailurile de ieșire care conțin anumite tipuri de informații sensibile din entitatea găzduită în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="2504a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="2504a-106">În schimb, vă oferim instrucțiuni detaliate despre modul în care puteți face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="2504a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="2504a-107">Pentru detalii suplimentare despre cum să creați o regulă de transport pentru a cripta informațiile sensibile, consultați [acest articol](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="2504a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="2504a-108">Dacă utilizați Outlook pe web (anterior **OWA**): atunci când compuneți un mesaj de e-mail, pur și simplu faceți clic pe **Protejare** în OWA.</span><span class="sxs-lookup"><span data-stu-id="2504a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="2504a-109">Se va aplica permisiunea "nu se redirecționează".</span><span class="sxs-lookup"><span data-stu-id="2504a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="2504a-110">Faceți clic pe **modificare permisiune** și alegeți **criptare** pentru a cripta doar mesajul.</span><span class="sxs-lookup"><span data-stu-id="2504a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="2504a-111">Dacă utilizați **clientul Outlook**: pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Options**  >  **permisiuni**de opțiuni, apoi selectați opțiunea de protecție de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="2504a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="2504a-112">Pentru a **cripta automat toate mesajele de e-mail** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport a fluxului de corespondență în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="2504a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="2504a-113">Instrucțiunile detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="2504a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

