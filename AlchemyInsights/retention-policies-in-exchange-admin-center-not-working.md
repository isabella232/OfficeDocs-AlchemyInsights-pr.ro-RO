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
# <a name="retention-policies-in-exchange-admin-center"></a>Politici de retenție în Centrul de administrare Exchange

Dacă doriți să executăm verificări automate pentru setările menționate mai jos, selectați butonul înapoi <-- în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu politicile de retenție.

 **Problemă:** Politicile de retenție nou create sau actualizate în Centrul de administrare Exchange nu se aplică cutiilor poștale sau elementele nu sunt mutate în cutia poștală de arhivă sau șterse. 
  
 **Cauzele:**
  
- Acest lucru se poate termina cu faptul că **Asistentul de foldere gestionate** nu a procesat cutia poștală a utilizatorului. Asistentul de foldere gestionate încearcă să proceseze fiecare cutie poștală din organizația dvs. Dacă modificați o etichetă de retenție sau aplicați o altă politică de retenție unei cutii poștale, aveți posibilitatea să așteptați până când Asistență folder gestionat procesează cutia poștală sau puteți executa cmdlet-ul Start-ManagedFolderAssistant pentru a porni Asistentul de foldere gestionate pentru a procesa o anumită cutie poștală. Executarea acestui cmdlet este utilă pentru testarea sau depanarea unei politici de retenție sau a setărilor etichetei de retenție. Pentru mai multe informații, vizitați [Executare Asistent folder gestionat](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Soluție:** Executați următoarea comandă pentru a porni Asistentul de foldere gestionate pentru o anumită cutie poștală:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Acest lucru poate apărea, de asemenea, dacă **RetentionHold** a fost **activat** pe cutia poștală. Dacă cutia poștală a fost plasată pe un RetentionHold, politica de retenție pe cutia poștală nu va fi procesată în acest timp. Pentru mai multe informații despre setarea RetentionHold consultați: [Păstrarea cutiei poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluţie:**
    
  - Verificați starea setării RetentionHold pe cutia poștală specifică în [powershell EXO:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Executați următoarea comandă pentru a **dezactiva** RetentionHold pe o anumită cutie poștală:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Acum, executați din nou Asistentul de foldere gestionate:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Notă:** Dacă o cutie poștală este mai mică de 10 MO, Asistentul de foldere gestionate nu va procesa automat cutia poștală.
 
Pentru mai multe informații despre politicile de retenție din Centrul de administrare Exchange, consultați:
- [Etichete de retenție și politici de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicarea unei politici de retenție la cutiile poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adăugarea sau eliminarea etichetelor de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [se identifică tipul de suspendare plasat pe o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
