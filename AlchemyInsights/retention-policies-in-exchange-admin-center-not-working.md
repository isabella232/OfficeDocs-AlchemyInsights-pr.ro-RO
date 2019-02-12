---
title: Strategiile de conservare în centrul de administrare Exchange nu de lucru
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935004"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="fe7af-102">Strategiile de conservare în centrul de administrare Exchange</span><span class="sxs-lookup"><span data-stu-id="fe7af-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="fe7af-103">**Problemă:** Nou create sau politicile de reţinere Actualizat în centrul de administrare Exchange sunt se aplică cutiilor poştale sau obiecte nu sunt mutate în cutia poştală de arhivă sau şters.</span><span class="sxs-lookup"><span data-stu-id="fe7af-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="fe7af-104">**Cauzele:**</span><span class="sxs-lookup"><span data-stu-id="fe7af-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="fe7af-p101">Acest lucru poate fi pentru că **Asistentul pentru foldere gestionate** nu a procesat cutia poştală a utilizatorului. Asistentul pentru foldere gestionate încearcă să proceseze fiecare cutie poştală din organizaţia din cadrul norului o dată la şapte zile. Dacă modificaţi o etichetă de conservare sau aplicaţi o diferite de conservare unei cutii poştale, puteţi să aşteptaţi până când a reuşit Folder asista procesează cutia poştală, sau aveţi posibilitatea să executaţi cmdletul Start-ManagedFolderAssistant pentru a porni asistentul pentru foldere gestionate să proceseze o anumită cutie poştală. Executarea acestui cmdlet este util pentru testare şi depanare o conservare sau setările de etichetă de conservare. Pentru mai multe informaţii, vizitaţi [rula asistentul pentru foldere gestionate](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="fe7af-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="fe7af-110">**Solutie:** Executaţi următoarea comandă pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poştală:</span><span class="sxs-lookup"><span data-stu-id="fe7af-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="fe7af-p102">Acest lucru poate fi produce în cazul în care **RetentionHold** a fost **activat** în cutia poştală. În cazul în care cutia poştală a fost plasat pe o RetentionHold, conservare în cutia poştală nu vor fi procesate în acea perioadă. Pentru legatura cu informaton mai multe pe RetentionHold setarea vedea: [Cutie poştală retenţie Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="fe7af-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="fe7af-114">**Soluţie:**</span><span class="sxs-lookup"><span data-stu-id="fe7af-114">**Solution:**</span></span>
    
  - <span data-ttu-id="fe7af-115">Verifica starea de setarea RetentionHold cutiei poştale specifice în [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="fe7af-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="fe7af-116">Executaţi următoarea comandă pentru **a dezactiva** RetentionHold pe o anumită cutie poştală:</span><span class="sxs-lookup"><span data-stu-id="fe7af-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="fe7af-117">Acum, re-a alerga folderul Managed asistent:</span><span class="sxs-lookup"><span data-stu-id="fe7af-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="fe7af-118">**Notă:** Dacă o cutie poştală este mai mică de 10 MB, asistentul pentru foldere gestionate va nu automat procesează cutia poştală.</span><span class="sxs-lookup"><span data-stu-id="fe7af-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

