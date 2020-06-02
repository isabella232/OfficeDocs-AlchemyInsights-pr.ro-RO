---
title: Politicile de conservare din Centrul de administrare Exchange nu funcționează
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
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502619"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politicile de conservare în Centrul de administrare Exchange

 **Problema:** Politicile de conservare nou create sau actualizate în Centrul de administrare Exchange nu se aplică cutiilor poștale sau elemente nu sunt mutate în cutia poștală arhivă sau șterse. 
  
 **Cauzele:**
  
- Acest lucru se poate datora faptului că **Asistentul de foldere gestionate** nu a procesat cutia poștală a utilizatorului. Asistentul folder gestionat încearcă să proceseze fiecare cutie poștală din organizația din cadrul norului o dată la fiecare șapte zile. Dacă modificați o etichetă de conservare sau aplicați o altă politică de conservare la o cutie poștală, aveți posibilitatea să așteptați până când Asistata de folder gestionat procesează cutia poștală sau aveți posibilitatea să executați cmdletul Start-ManagedFolderAssistant pentru a porni Asistentul folder gestionat pentru a procesa o anumită cutie poștală. Executarea acestui cmdlet este utilă pentru testarea sau depanarea unei politici de conservare sau a setărilor etichetei de conservare. Pentru mai multe informații, vizitați [Executare asistent folder gestionat](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Soluție:** Executați următoarea comandă pentru a porni Asistent folder gestionat pentru o anumită cutie poștală:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Acest lucru poate apărea, de asemenea, dacă **RetentionHold** a fost **activat** ă în cutia poștală. Dacă cutia poștală a fost plasat pe un RetentionHold, politica de retenție pe cutia poștală nu vor fi procesate în acest timp. Pentru mai multe informații despre setarea RetentionHold consultați: [Păstrare cutie poștală](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluţie:**
    
  - Verificați starea setării RetentionHold pe cutia poștală specifică în [exo powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Executați următoarea comandă pentru a **dezactiva** RetentionHold pe o anumită cutie poștală:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Acum, executați din nou asistentul folderului gestionat:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Notã:** Dacă o cutie poștală este mai mică de 10 MO, Asistentul folder gestionat nu va procesa automat cutia poștală.
 
Pentru mai multe informații despre politicile de conservare din Centrul de administrare Exchange, consultați:
- [Etichete de conservare și politici de conservare](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicarea unei politici de conservare pentru cutiile poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adăugarea sau eliminarea etichetelor de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [se identifică tipul de reținere plasat pe o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
