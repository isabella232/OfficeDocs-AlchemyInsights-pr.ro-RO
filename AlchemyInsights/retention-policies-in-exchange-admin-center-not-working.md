---
title: Strategiile de conservare în centrul de administrare Exchange nu de lucru
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761594"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="f2d6d-102">Strategiile de conservare în centrul de administrare Exchange</span><span class="sxs-lookup"><span data-stu-id="f2d6d-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="f2d6d-103">**Problemă:** Nou create sau politicile de reţinere Actualizat în centrul de administrare Exchange sunt se aplică cutiilor poştale sau obiecte nu sunt mutate în cutia poştală de arhivă sau şters.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="f2d6d-104">**Cauzele:**</span><span class="sxs-lookup"><span data-stu-id="f2d6d-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="f2d6d-105">Acest lucru poate fi pentru că **Asistentul pentru foldere gestionate** nu a procesat cutia poştală a utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="f2d6d-106">Asistentul pentru foldere gestionate încearcă să proceseze fiecare cutie poştală din organizaţia din cadrul norului o dată la şapte zile.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="f2d6d-107">Dacă modificaţi o etichetă de conservare sau aplicaţi o diferite de conservare unei cutii poştale, puteţi să aşteptaţi până când a reuşit Folder asista procesează cutia poştală, sau aveţi posibilitatea să executaţi cmdletul Start-ManagedFolderAssistant pentru a porni asistentul pentru foldere gestionate să proceseze o anumită cutie poştală.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="f2d6d-108">Executarea acestui cmdlet este util pentru testare şi depanare o conservare sau setările de etichetă de conservare.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="f2d6d-109">Pentru mai multe informaţii, vizitaţi [rula asistentul pentru foldere gestionate](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="f2d6d-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="f2d6d-110">**Solutie:** Executaţi următoarea comandă pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poştală:</span><span class="sxs-lookup"><span data-stu-id="f2d6d-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="f2d6d-111">Acest lucru poate fi produce în cazul în care **RetentionHold** a fost **activat** în cutia poştală.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="f2d6d-112">În cazul în care cutia poştală a fost plasat pe o RetentionHold, conservare în cutia poştală nu vor fi procesate în acea perioadă.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="f2d6d-113">Pentru legatura cu informaton mai multe pe RetentionHold setarea vedea: [Cutie poştală retenţie Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="f2d6d-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="f2d6d-114">**Soluţie:**</span><span class="sxs-lookup"><span data-stu-id="f2d6d-114">**Solution:**</span></span>
    
  - <span data-ttu-id="f2d6d-115">Verifica starea de setarea RetentionHold cutiei poştale specifice în [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="f2d6d-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="f2d6d-116">Executaţi următoarea comandă pentru **a dezactiva** RetentionHold pe o anumită cutie poştală:</span><span class="sxs-lookup"><span data-stu-id="f2d6d-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="f2d6d-117">Acum, re-a alerga folderul Managed asistent:</span><span class="sxs-lookup"><span data-stu-id="f2d6d-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="f2d6d-118">**Notă:** Dacă o cutie poştală este mai mică de 10 MB, asistentul pentru foldere gestionate va nu automat procesează cutia poştală.</span><span class="sxs-lookup"><span data-stu-id="f2d6d-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

