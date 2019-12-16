---
title: S/MIME în Outlook pe web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053237"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="75b6a-102">Criptarea mesajelor de e-mail în Outlook</span><span class="sxs-lookup"><span data-stu-id="75b6a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="75b6a-103">Office 365 mesaj Encryption este construit pe Microsoft Azure Rights Management (Azure RMS), care face parte din protecție informații Azure.</span><span class="sxs-lookup"><span data-stu-id="75b6a-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="75b6a-104">Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu trebuie să efectuați nicio acțiune pentru a activa sau activa manual** serviciul de administrare a drepturilor.</span><span class="sxs-lookup"><span data-stu-id="75b6a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="75b6a-105">Pe baza feedback-ului clientului, nu vom mai permite regulilor de flux de corespondență Exchange să cripteze automat e-mailul de ieșire care conține anumite tipuri de informații sensibile în entitatea găzduită în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="75b6a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="75b6a-106">În schimb, oferim instrucțiuni detaliate despre puteți face acest lucru.</span><span class="sxs-lookup"><span data-stu-id="75b6a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="75b6a-107">Pentru detalii suplimentare despre să creați o regulă de transport pentru a cripta informații sensibile, consultați [acest articol](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="75b6a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="75b6a-108">Dacă utilizați Outlook pe web (fostă **OWA**): Când compuneți un mesaj de poștă electronică, pur și simplu faceți clic pe **Protejare** în OWA.</span><span class="sxs-lookup"><span data-stu-id="75b6a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="75b6a-109">Acest lucru va aplica permisiunea "nu redirecționați".</span><span class="sxs-lookup"><span data-stu-id="75b6a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="75b6a-110">Faceți clic pe **modificare permisiune** și alegeți **criptare** pentru a cripta numai mesajul.</span><span class="sxs-lookup"><span data-stu-id="75b6a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="75b6a-111">Dacă utilizați **clientul Outlook**: pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Opțiuni** > **permisiuni**, apoi selectați opțiunea de protecție de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="75b6a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="75b6a-112">Pentru a **cripta automat toate mesajele de poștă electronică** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport flux de corespondență în centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="75b6a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="75b6a-113">Instrucțiuni detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="75b6a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

