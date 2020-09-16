---
title: Politicile de retenție din centrul de administrare Exchange nu funcționează
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
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740522"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="7b213-102">Politici de retenție în centrul de administrare Exchange</span><span class="sxs-lookup"><span data-stu-id="7b213-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="7b213-103">Dacă doriți ca noi să efectuăm verificări automate pentru setările menționate mai jos, selectați butonul înapoi <-în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu politicile de retenție.</span><span class="sxs-lookup"><span data-stu-id="7b213-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="7b213-104">**Problemă:** Politicile de retenție nou create sau actualizate din centrul de administrare Exchange nu se aplică la cutiile poștale sau elementele nu sunt mutate în cutia poștală de arhivă sau sunt șterse.</span><span class="sxs-lookup"><span data-stu-id="7b213-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="7b213-105">**Cauzele rădăcină:**</span><span class="sxs-lookup"><span data-stu-id="7b213-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="7b213-106">Acest lucru se poate datora faptului că **Asistentul pentru foldere gestionate** nu a procesat cutia poștală a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="7b213-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="7b213-107">Asistentul pentru foldere gestionate încearcă să proceseze fiecare cutie poștală din organizația bazată pe cloud o dată la șapte zile.</span><span class="sxs-lookup"><span data-stu-id="7b213-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="7b213-108">Dacă modificați o etichetă de retenție sau aplicați o politică de retenție diferită la o cutie poștală, puteți aștepta până când folderul gestionat asistă procesele cutiei poștale sau puteți rula cmdletul Start-ManagedFolderAssistant pentru a porni asistentul pentru foldere gestionate pentru a procesa o anumită cutie poștală.</span><span class="sxs-lookup"><span data-stu-id="7b213-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="7b213-109">Executarea acestui cmdlet este utilă pentru testarea sau depanarea unei politici de retenție sau a setărilor etichetei de retenție.</span><span class="sxs-lookup"><span data-stu-id="7b213-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="7b213-110">Pentru mai multe informații, vizitați [rulează asistentul pentru foldere gestionate](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="7b213-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="7b213-111">**Soluție:** Rulează următoarea comandă pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="7b213-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="7b213-112">Acest lucru se poate întâmpla și dacă **RetentionHold** a fost **activat** în cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="7b213-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="7b213-113">Dacă cutia poștală a fost plasată pe o RetentionHold, Politica de retenție din cutia poștală nu va fi procesată în acel moment.</span><span class="sxs-lookup"><span data-stu-id="7b213-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="7b213-114">Pentru mai multe Informaton în setarea RetentionHold, consultați: reținerea [cutiei poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="7b213-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="7b213-115">**Soluție**</span><span class="sxs-lookup"><span data-stu-id="7b213-115">**Solution:**</span></span>
    
  - <span data-ttu-id="7b213-116">Verificați starea setării RetentionHold din cutia poștală specifică din [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="7b213-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="7b213-117">Rulează următoarea comandă pentru a **dezactiva** RetentionHold pe o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="7b213-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="7b213-118">Acum, Reexecutați asistentul pentru foldere gestionate:</span><span class="sxs-lookup"><span data-stu-id="7b213-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="7b213-119">**Notă:** Dacă o cutie poștală este mai mică decât 10 MB, asistentul pentru foldere gestionate nu va procesa automat cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="7b213-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="7b213-120">Pentru mai multe informații despre politicile de retenție din centrul de administrare Exchange, consultați:</span><span class="sxs-lookup"><span data-stu-id="7b213-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="7b213-121">Etichete de retenție și politici de retenție</span><span class="sxs-lookup"><span data-stu-id="7b213-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="7b213-122">Aplicarea unei politici de retenție pentru cutiile poștale</span><span class="sxs-lookup"><span data-stu-id="7b213-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="7b213-123">Adăugarea sau eliminarea etichetelor de retenție</span><span class="sxs-lookup"><span data-stu-id="7b213-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="7b213-124">Cum se identifică tipul de reținere plasat într-o cutie poștală</span><span class="sxs-lookup"><span data-stu-id="7b213-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
