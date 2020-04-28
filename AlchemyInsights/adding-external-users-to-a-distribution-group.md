---
title: Adăugarea utilizatorilor externi la un grup de distribuire
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910944"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adăugarea utilizatorilor externi la un grup de distribuire

Adăugarea unui contact extern la un grup de distribuire (DG) este un proces în doi pași:
  
1. Crearea unei persoane de contact de poștă electronică pentru utilizatorul extern:
    
    1. În centrul de administrare, accesați pagina[Persoane de contact](https://admin.microsoft.com/adminportal/home#/Contact) **utilizatori.** >  
    
    2. Selectați **Adăugare persoană de contact**.
    
    3. Tastați informațiile pentru persoana de contact și selectați **Adăugare**.
    
2. Adăugați contactul de poștă electronică la DG:
    
    1. În centrul de administrare, accesați pagina **Grupuri** > [grupuri.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Găsiți DG-ul la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide dialogul de editare.
    
    3. În fila **Membri,** selectați **Vizualizare totală și gestionare membri**. 
    
    4. Selectați **Adăugare membri**.
    
    5. Selectați contactul de poștă electronică pe care l-ați creat la pasul anterior, apoi selectați **Salvare**.
    
Dacă după ce urmați acești pași, utilizatorii externi nu pot trimite e-mailuri către DG sau nu primesc e-mailuri de la acesta, este posibil ca DG să fie marcată pentru a permite numai e-mailuri de la utilizatori interni. Puteți verifica această configurație și fixați-l urmând instrucțiunile [de aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Notã:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "Microsoft 365 group" în loc de "Grup de distribuire". Dacă acesta este cazul, puteți adăuga utilizatorul extern direct la grupul din Outlook. Informații detaliate despre Microsoft 365 Groups guests as well as instructions for adding external guests pot fi găsite în [acest articol](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  