---
title: Strategiile de conservare în centrul de administrare Exchange nu de lucru
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306636"
---
 **Problemă:** Nou create sau politicile de reţinere Actualizat în centrul de administrare Exchange sunt se aplică cutiilor poştale sau obiecte nu sunt mutate în cutia poştală de arhivă sau şters. 
  
 **Cauzele:**
  
- Acest lucru poate fi pentru că **Asistentul pentru foldere gestionate** nu a procesat cutia poştală a utilizatorului. Asistentul pentru foldere gestionate încearcă să proceseze fiecare cutie poştală din organizaţia din cadrul norului o dată la şapte zile. Dacă modificaţi o etichetă de conservare sau aplicaţi o diferite de conservare unei cutii poştale, puteţi să aşteptaţi până când a reuşit Folder asista procesează cutia poştală, sau aveţi posibilitatea să executaţi cmdletul Start-ManagedFolderAssistant pentru a porni asistentul pentru foldere gestionate să proceseze o anumită cutie poştală. Executarea acestui cmdlet este util pentru testare şi depanare o conservare sau setările de etichetă de conservare. Pentru mai multe informaţii, vizitaţi [rula asistentul pentru foldere gestionate](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solutie:** Executaţi următoarea comandă pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poştală: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Acest lucru poate fi produce în cazul în care **RetentionHold** a fost **activat** în cutia poştală. În cazul în care cutia poştală a fost plasat pe o RetentionHold, conservare în cutia poştală nu vor fi procesate în acea perioadă. Pentru legatura cu informaton mai multe pe RetentionHold setarea vedea: [Cutie poştală retenţie Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluţie:**
    
  - Verifica starea de setarea RetentionHold cutiei poştale specifice în [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Executaţi următoarea comandă pentru **a dezactiva** RetentionHold pe o anumită cutie poştală: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Acum, re-a alerga folderul Managed asistent:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Notă:** Dacă o cutie poştală este mai mică de 10 MB, asistentul pentru foldere gestionate va nu automat procesează cutia poştală. 
  

