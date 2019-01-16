---
title: Muta mesajele de e-mail către cutia poştală de arhivă
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28307707"
---
Probleme de arhivare elementele în cutia poştală de arhivă. Asiguraţi-vă că aţi parcurs paşii de mai jos:
  
1. Confirmaţi că o **Arhiva cutie poştală** a fost activată. Dacă nu, utilizaţi paşii din [acest articol](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) pentru a permite cutiei poştale de arhivă. 
    
2. În centrul de administrare Exchange, selectaţi **Etichetele de conservare** , sub **Managementul de conformitate**, creaţi o **etichetă de conservare** cu acţiunea **trece la Arhiva** conţinând dorit de **Vechime de conservare**.
    
3. În centrul de administrare Exchange, selectaţi **Strategiile de conservare**, crea o **Strategie de conservare** şi se adaugă vă **trece la Arhiva** etichetă de conservare a acestei politici. 
    
4. [Atribui conservare](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) la cutia poştală a utilizatorului specifice. Aceeaşi politică va aplica atât **primare** şi cutia poştală de **arhivă** . 
    
Cutia poştală a utilizatorului acum ar trebui să aibă o politică de Arhiva să mutaţi elementele în cutia poştală de arhivă. Este necesar să se vigoare reuşit Folder asistent (MAE) pentru a rula şi de a aplica noile setări pentru cutia poştală a utilizatorului. Executaţi următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poştală: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Doresc mai multe informaţii privind înfiinţarea unei politici de arhiva, a se vedea [Configurarea unei politici Arhiva şi ştergere pentru cutii poştale](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

