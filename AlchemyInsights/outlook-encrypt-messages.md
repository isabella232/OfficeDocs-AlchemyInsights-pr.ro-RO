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
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764884"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="f0fea-102">Criptarea mesajelor de e-mail în Outlook</span><span class="sxs-lookup"><span data-stu-id="f0fea-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="f0fea-103">Microsoft 365 mesaj criptare este construit pe Microsoft Azure Rights Management (Azure RMS), care face parte din Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="f0fea-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="f0fea-104">Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu este necesar să efectuați nicio acțiune pentru a activa sau activa manual** Serviciul de gestionare a drepturilor.</span><span class="sxs-lookup"><span data-stu-id="f0fea-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="f0fea-105">Pe baza feedback-ului clientului, nu vom mai permite regulilor fluxului de corespondență Exchange să cripteze automat e-mailul de ieșire care conține anumite tipuri de informații sensibile din entitatea găzduită în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="f0fea-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="f0fea-106">În schimb, oferim instrucțiuni detaliate cu privire la modul în care puteți face acest lucru voi înșivă.</span><span class="sxs-lookup"><span data-stu-id="f0fea-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="f0fea-107">Pentru detalii suplimentare despre se creează o regulă de transport pentru a cripta informațiile sensibile, consultați [acest articol](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="f0fea-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="f0fea-108">Dacă utilizați Outlook pe Web (anterior **OWA**): Atunci când compuneți un mesaj de poștă electronică, pur și simplu faceți clic pe **Protejaîn** OWA.</span><span class="sxs-lookup"><span data-stu-id="f0fea-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="f0fea-109">Acest lucru se va aplica "Nu înainte" permisiunea.</span><span class="sxs-lookup"><span data-stu-id="f0fea-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="f0fea-110">Faceți clic pe **Modificare permisiune** și **alegeți Criptare** pentru a cripta numai mesajul.</span><span class="sxs-lookup"><span data-stu-id="f0fea-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="f0fea-111">Dacă utilizați **clientul Outlook**: Pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Permisiuni de opțiuni** > **Permissions**, apoi selectați opțiunea de protecție de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="f0fea-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="f0fea-112">Pentru a **cripta automat toate e-mailurile** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport flux de corespondență în Centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0fea-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="f0fea-113">Instrucțiuni detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="f0fea-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

