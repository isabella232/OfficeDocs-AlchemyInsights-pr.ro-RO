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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511520"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="e035f-102">Criptarea mesajelor de e-mail în Outlook</span><span class="sxs-lookup"><span data-stu-id="e035f-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="e035f-103">Microsoft 365 mesaj criptare este construit pe Microsoft Azure Rights Management (Azure RMS), care face parte din Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="e035f-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="e035f-104">Dacă abonamentul include Azure Rights Management sau Azure Information Protection, **nu este necesar să efectuați nicio acțiune pentru a activa sau activa manual** Serviciul de gestionare a drepturilor.</span><span class="sxs-lookup"><span data-stu-id="e035f-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="e035f-105">Pe baza feedback-ului clientului, nu vom mai permite regulilor fluxului de corespondență Exchange să cripteze automat e-mailul de ieșire care conține anumite tipuri de informații sensibile din entitatea găzduită în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="e035f-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="e035f-106">În schimb, oferim instrucțiuni detaliate cu privire la modul în care puteți face acest lucru voi înșivă.</span><span class="sxs-lookup"><span data-stu-id="e035f-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="e035f-107">Pentru detalii suplimentare despre se creează o regulă de transport pentru a cripta informațiile sensibile, consultați [acest articol](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="e035f-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="e035f-108">Dacă utilizați Outlook pe Web (anterior **OWA**): Atunci când compuneți un mesaj de poștă electronică, pur și simplu faceți clic pe **Protejaîn** OWA.</span><span class="sxs-lookup"><span data-stu-id="e035f-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="e035f-109">Acest lucru se va aplica "Nu înainte" permisiunea.</span><span class="sxs-lookup"><span data-stu-id="e035f-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="e035f-110">Faceți clic pe **Modificare permisiune** și **alegeți Criptare** pentru a cripta numai mesajul.</span><span class="sxs-lookup"><span data-stu-id="e035f-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="e035f-111">Dacă utilizați **clientul Outlook**: Pentru a trimite un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectați **Permisiuni de opțiuni**, apoi  >  **Permissions**selectați opțiunea de protecție de care aveți nevoie.</span><span class="sxs-lookup"><span data-stu-id="e035f-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="e035f-112">Pentru a **cripta automat toate e-mailurile** trimise anumitor destinatari sau organizații partenere externe, trebuie să creați o regulă de transport flux de corespondență în Centrul de administrare Exchange.</span><span class="sxs-lookup"><span data-stu-id="e035f-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="e035f-113">Instrucțiuni detaliate sunt furnizate în [acest articol de asistență](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="e035f-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

