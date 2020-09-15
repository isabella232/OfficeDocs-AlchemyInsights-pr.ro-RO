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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663525"
---
# <a name="add-external-users-to-a-distribution-group"></a>Adăugarea utilizatorilor externi la un grup de distribuire

Adăugarea unei persoane de contact externe la un grup de distribuire (DG) este un proces în doi pași:
  
1. Creați o persoană de contact de E-mail pentru utilizatorul extern:
    
    1. În centrul de administrare, accesați **Users**  >  pagina[persoane de contact](https://admin.microsoft.com/adminportal/home#/Contact) pentru utilizatori. 
    
    2. Selectați **Adăugați o persoană de contact**.
    
    3. Tastați informațiile pentru persoana de contact și selectați **Adăugare**.
    
2. Adăugați persoana de contact de E-mail la DG:
    
    1. În centrul de administrare, accesați pagina grupuri **grupuri**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Găsiți DG-ul la care doriți să adăugați utilizatorul extern și selectați-l pentru a deschide caseta de dialog Editare.
    
    3. Pe fila **Membri** , selectați **Vizualizați toți și gestionați membri**. 
    
    4. Selectați **Adăugare membri**.
    
    5. Selectați persoana de contact de E-mail pe care ați creat-o la pasul anterior, apoi selectați **Salvare**.
    
Dacă după ce urmați acești pași, utilizatorii externi nu pot trimite mesaje de e-mail către DG sau nu primesc mesaje de e-mail de la acesta, ar putea fi faptul că DG este marcată pentru a permite doar mesajele de e-mail de la utilizatorii interni. Puteți să verificați această configurație și să o remediați urmând instrucțiunile de [aici](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Notă:** Aceste instrucțiuni nu se aplică dacă tipul grupului este "Microsoft 365 Group" în loc de "grup de distribuire". Dacă acesta este cazul, puteți adăuga utilizatorul extern direct la grup din Outlook. Informații detaliate despre Microsoft 365 Groups invitati, precum și instrucțiuni pentru adăugarea oaspeților externi pot fi găsiți în [acest articol](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  