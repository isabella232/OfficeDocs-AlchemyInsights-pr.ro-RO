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
# <a name="retention-policies-in-exchange-admin-center"></a>Politici de retenție în centrul de administrare Exchange

Dacă doriți ca noi să efectuăm verificări automate pentru setările menționate mai jos, selectați butonul înapoi <-în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu politicile de retenție.

 **Problemă:** Politicile de retenție nou create sau actualizate din centrul de administrare Exchange nu se aplică la cutiile poștale sau elementele nu sunt mutate în cutia poștală de arhivă sau sunt șterse. 
  
 **Cauzele rădăcină:**
  
- Acest lucru se poate datora faptului că **Asistentul pentru foldere gestionate** nu a procesat cutia poștală a utilizatorului. Asistentul pentru foldere gestionate încearcă să proceseze fiecare cutie poștală din organizația bazată pe cloud o dată la șapte zile. Dacă modificați o etichetă de retenție sau aplicați o politică de retenție diferită la o cutie poștală, puteți aștepta până când folderul gestionat asistă procesele cutiei poștale sau puteți rula cmdletul Start-ManagedFolderAssistant pentru a porni asistentul pentru foldere gestionate pentru a procesa o anumită cutie poștală. Executarea acestui cmdlet este utilă pentru testarea sau depanarea unei politici de retenție sau a setărilor etichetei de retenție. Pentru mai multe informații, vizitați [rulează asistentul pentru foldere gestionate](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Soluție:** Rulează următoarea comandă pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poștală:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Acest lucru se poate întâmpla și dacă **RetentionHold** a fost **activat** în cutia poștală. Dacă cutia poștală a fost plasată pe o RetentionHold, Politica de retenție din cutia poștală nu va fi procesată în acel moment. Pentru mai multe Informaton în setarea RetentionHold, consultați: reținerea [cutiei poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Soluție**
    
  - Verificați starea setării RetentionHold din cutia poștală specifică din [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Rulează următoarea comandă pentru a **dezactiva** RetentionHold pe o anumită cutie poștală:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Acum, Reexecutați asistentul pentru foldere gestionate:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Notă:** Dacă o cutie poștală este mai mică decât 10 MB, asistentul pentru foldere gestionate nu va procesa automat cutia poștală.
 
Pentru mai multe informații despre politicile de retenție din centrul de administrare Exchange, consultați:
- [Etichete de retenție și politici de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Aplicarea unei politici de retenție pentru cutiile poștale](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Adăugarea sau eliminarea etichetelor de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Cum se identifică tipul de reținere plasat într-o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
