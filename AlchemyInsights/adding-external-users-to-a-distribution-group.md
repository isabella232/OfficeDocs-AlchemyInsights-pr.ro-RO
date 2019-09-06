---
title: Adăugarea de utilizatori externi la un grup de distribuire
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737885"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adăugarea de utilizatori externi la un grup de distribuire

Adăugarea unui contact extern la un grup de distribuire (DG) este un proces în două etape:
  
1. Creați o persoană de contact de poștă electronică pentru utilizatorul extern:
    
    1. În centrul de administrare, accesați pagina contacte **utilizatori** > [](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Selectați **Adăugați un contact**.
    
    3. Tastați informațiile pentru persoana de contact și selectați **Adăugare**.
    
2. Adăugați contactul de poștă electronică la DG-ul dvs.:
    
    1. În centrul de administrare, accesați > pagina[grupuri](https://admin.microsoft.com/adminportal/home#/groups) grupuri. **** 
    
    2. Găsiți DG la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide dialogul de editare.
    
    3. În fila **Membri** , selectați **Vizualizați toți și gestionați membrii**. 
    
    4. Selectați **Adăugați membri**.
    
    5. Selectați contactul de poștă electronică pe care l-ați creat în pasul anterior, apoi selectați **Salvare**.
    
Dacă după ce urmați acești pași utilizatorii externi nu pot trimite e-mailuri la DG sau nu primesc e-mailuri de la ea, ar putea fi că DG este marcat pentru a permite numai e-mailuri de la utilizatorii interni. Puteți verifica această configurație și fixați-o urmând instrucțiunile de [aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Notă:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "Office 365 Group" în loc de "grup de distribuire". În acest caz, aveți posibilitatea să adăugați utilizatorul extern direct la grupul din Outlook. Informații detaliate cu privire la Office 365 grupuri de oaspeți, precum și instrucțiuni pentru adăugarea de oaspeți externi pot fi găsite în [acest articol](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  