---
title: Politicile de retenție din Centrul de administrare Exchange nu funcționează
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522819"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="6164a-102">Politici de retenție în Centrul de administrare Exchange</span><span class="sxs-lookup"><span data-stu-id="6164a-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="6164a-103">Dacă doriți să executăm verificări automate pentru setările menționate mai jos, selectați butonul înapoi <-- în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu politicile de retenție.</span><span class="sxs-lookup"><span data-stu-id="6164a-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="6164a-104">**Problemă:** Politicile de retenție nou create sau actualizate în Centrul de administrare Exchange nu se aplică cutiilor poștale sau elementele nu sunt mutate în cutia poștală de arhivă sau șterse.</span><span class="sxs-lookup"><span data-stu-id="6164a-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="6164a-105">**Cauzele:**</span><span class="sxs-lookup"><span data-stu-id="6164a-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="6164a-106">Acest lucru se poate termina cu faptul că **Asistentul de foldere gestionate** nu a procesat cutia poștală a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="6164a-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="6164a-107">Asistentul de foldere gestionate încearcă să proceseze fiecare cutie poștală din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="6164a-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="6164a-108">Dacă modificați o etichetă de retenție sau aplicați o altă politică de retenție unei cutii poștale, aveți posibilitatea să așteptați până când Asistență folder gestionat procesează cutia poștală sau puteți executa cmdlet-ul Start-ManagedFolderAssistant pentru a porni Asistentul de foldere gestionate pentru a procesa o anumită cutie poștală.</span><span class="sxs-lookup"><span data-stu-id="6164a-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="6164a-109">Executarea acestui cmdlet este utilă pentru testarea sau depanarea unei politici de retenție sau a setărilor etichetei de retenție.</span><span class="sxs-lookup"><span data-stu-id="6164a-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="6164a-110">Pentru mai multe informații, vizitați [Executare Asistent folder gestionat](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="6164a-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="6164a-111">**Soluție:** Executați următoarea comandă pentru a porni Asistentul de foldere gestionate pentru o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="6164a-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="6164a-112">Acest lucru poate apărea, de asemenea, dacă **RetentionHold** a fost **activat** pe cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="6164a-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="6164a-113">Dacă cutia poștală a fost plasată pe un RetentionHold, politica de retenție pe cutia poștală nu va fi procesată în acest timp.</span><span class="sxs-lookup"><span data-stu-id="6164a-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="6164a-114">Pentru mai multe informații despre setarea RetentionHold consultați: [Păstrarea cutiei poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="6164a-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="6164a-115">**Soluţie:**</span><span class="sxs-lookup"><span data-stu-id="6164a-115">**Solution:**</span></span>
    
  - <span data-ttu-id="6164a-116">Verificați starea setării RetentionHold pe cutia poștală specifică în [powershell EXO:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="6164a-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="6164a-117">Executați următoarea comandă pentru a **dezactiva** RetentionHold pe o anumită cutie poștală:</span><span class="sxs-lookup"><span data-stu-id="6164a-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="6164a-118">Acum, executați din nou Asistentul de foldere gestionate:</span><span class="sxs-lookup"><span data-stu-id="6164a-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="6164a-119">**Notă:** Dacă o cutie poștală este mai mică de 10 MO, Asistentul de foldere gestionate nu va procesa automat cutia poștală.</span><span class="sxs-lookup"><span data-stu-id="6164a-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="6164a-120">Pentru mai multe informații despre politicile de retenție din Centrul de administrare Exchange, consultați:</span><span class="sxs-lookup"><span data-stu-id="6164a-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="6164a-121">Etichete de retenție și politici de retenție</span><span class="sxs-lookup"><span data-stu-id="6164a-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="6164a-122">Aplicarea unei politici de retenție la cutiile poștale</span><span class="sxs-lookup"><span data-stu-id="6164a-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="6164a-123">Adăugarea sau eliminarea etichetelor de retenție</span><span class="sxs-lookup"><span data-stu-id="6164a-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="6164a-124">se identifică tipul de suspendare plasat pe o cutie poștală</span><span class="sxs-lookup"><span data-stu-id="6164a-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
