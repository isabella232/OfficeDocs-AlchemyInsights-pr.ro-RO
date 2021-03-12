---
title: Depanarea mesajelor interzise în Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704906"
---
# <a name="troubleshoot-access-denied-messages"></a>Depanarea mesajelor interzise în Access

Dacă cineva a primit un mesaj "acces refuzat" la un folder partajat din SharePoint, este posibil ca administratorul colecției de site-uri să fi activat "modul de blocare a permisiunii pentru utilizatorul Access limitat". Pentru a dezactiva această problemă: 
  
1. Navigați la site, faceți clic pe pictograma Setări, apoi faceți clic pe **Setări site**.
    
2. Sub **Administrare colecție de site-uri**, faceți clic pe **Caracteristici colecție de site-uri**.
    
3. Lângă **modul blocare permisiune utilizator cu acces limitat**, faceți clic pe **Dezactivare**.
    
De asemenea, se poate produce un mesaj de acces refuzat pentru folderele partajate, dacă site-ul este un site de publicare. Pentru informații, consultați [Access Denied atunci când accesați un folder partajat](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Dacă o persoană a primit un mesaj "acces refuzat" atunci când încercați să vizualizați solicitările de acces, utilizatorul trebuie să fie adăugat ca administrator al colecției de site-uri sau ca membru al grupului de proprietari pentru site. Pentru mai multe informații, consultați [lista de solicitări Access Denied în Access](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Dacă un utilizator a primit un mesaj "acces refuzat" după ce a fost eliminat din Active Directory local, apoi s-a adăugat înapoi, consultați [Access Denied când un cont de utilizator este sincronizat la Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

