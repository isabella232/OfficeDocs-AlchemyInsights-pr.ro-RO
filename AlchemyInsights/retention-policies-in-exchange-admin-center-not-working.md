---
title: Politicile de retenție din Centrul de administrare Exchange nu funcționează
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952240"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="4cb9d-102">Politicile de retenție în Centrul de administrare Exchange</span><span class="sxs-lookup"><span data-stu-id="4cb9d-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="4cb9d-103">Dacă doriți să rulam verificări automate pentru setările menționate mai jos, selectați butonul Înapoi < - în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu politicile de retenție.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="4cb9d-104">Dacă aveți probleme cu politicile de conservare din Centrul de administrare Exchange care nu se aplică la cutiile poștale sau elementele care nu se mută în cutia poștală de arhivare, verificați următoarele:</span><span class="sxs-lookup"><span data-stu-id="4cb9d-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="4cb9d-105">**Cauze rădăcină:**</span><span class="sxs-lookup"><span data-stu-id="4cb9d-105">**Root Causes:**</span></span>

- <span data-ttu-id="4cb9d-106">**Asistentul de foldere gestionate** nu a procesat cutia poștală a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="4cb9d-107">Asistentul de foldere gestionate încearcă să proceseze fiecare cutie poștală din organizația dvs. bazată pe cloud o dată la șapte zile.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="4cb9d-108">**Soluție:** Rulați Asistentul de foldere gestionate.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="4cb9d-109">**Reținerea a** fost **activată pentru cutia** poștală.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="4cb9d-110">Dacă cutia poștală a fost plasată pe o Reținere de retenție, politica de reținere pentru cutia poștală nu va fi procesată în acest timp.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="4cb9d-111">**Soluție:** Verificați starea setării Reținere în așteptare și actualizați după cum este necesar.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="4cb9d-112">Pentru detalii, consultați Reținerea în așteptare [a cutiei poștale.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="4cb9d-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="4cb9d-113">**Notă:** Dacă o cutie poștală este mai mică de 10 MB, Asistentul de foldere gestionate nu va procesa automat cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="4cb9d-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="4cb9d-114">Pentru mai multe informații despre politicile de retenție din Centrul de administrare Exchange, consultați:</span><span class="sxs-lookup"><span data-stu-id="4cb9d-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="4cb9d-115">Etichetele de retenție și politicile de retenție</span><span class="sxs-lookup"><span data-stu-id="4cb9d-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="4cb9d-116">[Aplicarea unei politici de retenție pentru cutiile poștale sau](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Adăugarea sau eliminarea etichetelor de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="4cb9d-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="4cb9d-117">Cum să identificați tipul de așteptare plasat pe o cutie poștală</span><span class="sxs-lookup"><span data-stu-id="4cb9d-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
