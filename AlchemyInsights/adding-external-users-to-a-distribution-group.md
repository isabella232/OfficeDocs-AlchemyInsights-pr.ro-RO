---
title: Adăugarea utilizatorilor externi la un grup de distribuire
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934845"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adăugarea utilizatorilor externi la un grup de distribuire

Adăugarea unei persoane de contact externe la un grup de distribuire este un proces în doi pasul:
  
1. Crearea unei persoane de contact de e-mail pentru utilizatorul extern:
    
    1. În centrul de administrare, accesați pagina Persoane **de**  >  [contact utilizatori.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Selectați **Adăugați o persoană de contact**.
    
    3. Tastați informațiile pentru persoana de contact și selectați **Adăugare**.
    
2. Adăugarea persoanei de contact de e-mail la
    
    1. În centrul de administrare, accesați **pagina**  >  [Grupuri.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Găsiți programul de partajare la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide caseta de dialog Editare.
    
    3. Pe fila **Membri,** selectați Vedeți **tot și gestionați membrii**. 
    
    4. Selectați **Adăugați membri**.
    
    5. Selectați Persoana de contact de e-mail pe care ați creat-o la pasul anterior, apoi **selectați Salvare**.
    
Dacă, după ce urmați acești pași, utilizatorii externi nu pot trimite mesaje de e-mail către acesta sau nu primesc mesaje de e-mail de la acesta, cauza poate fi faptul că acesta este marcat pentru a permite doar mesaje de e-mail de la utilizatorii interni. Puteți să verificați această configurație și să o remediați urmând instrucțiunile [de aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Notă:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "grup Microsoft 365 grup" în loc de "Grup de distribuire". În acest caz, puteți adăuga utilizatorul extern direct la grup din Outlook. Informații detaliate despre Microsoft 365, precum și instrucțiuni pentru adăugarea invitaților externi pot fi găsite [în acest articol.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  