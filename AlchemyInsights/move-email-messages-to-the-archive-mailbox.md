---
title: Muta mesajele de e-mail către cutia poştală de arhivă
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418337"
---
# <a name="move-email-to-the-archive-mailbox"></a>Muta e-mail către cutia poştală de arhivă
 
1. Confirmaţi că o **Arhiva cutie poştală** a fost activată. Dacă nu, utilizaţi paşii din [acest articol](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pentru a permite cutiei poştale de arhivă.

2. Pentru a arhiva mesajele automat către cutia poştală de arhivă, o etichetă de conservare cu acţiunea **trece la Arhiva** trebuie setat aplică **automat întreaga cutie poştală (implicit) Tag-ul**. Utilizaţi paşii de aici pentru a crea Tag-ul: [implicit Arhiva tag-ul](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Apoi, Adăugaţi tag-ul **Arhiva** ta de conservare. În centrul de administrare Exchange, selectaţi **Strategiile de conservare** > adăuga **trece la Arhiva tag-ul** la > Politica de **Salvare**. 
    
4. Acum [aloca conservare](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cutia poştală a utilizatorului specifice. Aceeaşi politică va aplica atât **primare** şi cutia poştală de **arhivă** . 
    
Este necesar să se vigoare reuşit Folder asistent (MAE) pentru a rula şi de a aplica noile setări pentru cutia poştală a utilizatorului. Executaţi următoarea comandă în timp ce [conectat la EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pentru a porni asistentul pentru foldere gestionate pentru o anumită cutie poştală: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Pentru mai multe informaţii despre crearea unei politici de arhiva, a se vedea [Configurarea unei politici Arhiva şi ştergere pentru cutii poştale](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

