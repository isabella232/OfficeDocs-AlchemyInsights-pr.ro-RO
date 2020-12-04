---
title: Cum se adaugă sau se elimină un delegat în Outlook pentru Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573573"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Cum se adaugă sau se elimină un delegat în Outlook pentru Windows

Pentru a adăuga un delegat în Outlook pentru Windows: 

1. Faceți clic pe fila **fișier** , urmată de **setările contului**, apoi alegeți **delegare acces**.
2. Faceți clic pe **Adăugare**. Dacă **Add** nu apare, este posibil să nu existe o conexiune activă între Outlook și Exchange. Bara de stare Outlook afișează starea conexiunii.
3. Tastați numele persoanei pe care doriți să o desemnați ca delegat sau căutați și alegeți numele în lista cu rezultatele căutării.

    > [!NOTE]
    > Delegatul trebuie să fie o persoană din lista globală de adrese Exchange a Organizației (GAL).
4. Faceți clic pe **Add** urmat de **OK**.
5. În caseta de dialog **permisiuni delegat** , acceptați setările implicite de permisiune sau selectați niveluri de acces particularizate pentru folderele Exchange.

    - Dacă un delegat are nevoie de permisiune pentru a lucra doar cu solicitările de întâlnire și răspunsurile, setările de permisiune implicite, cum ar fi **delegat, primesc copii ale mesajelor asociate întâlnirii** sunt suficiente. Puteți să lăsați setarea permisiune **Inbox** la **fără**. Solicitările de întâlnire și răspunsurile vor merge direct la Inbox-ul delegat-ului.

    > [!NOTE]
    > În mod implicit, delegatul i se acordă **Editor (poate să citească, să creeze și să modifice elemente)** în folderul **Calendar** . Atunci când delegat răspunde la o întâlnire în numele dvs., acesta este adăugat automat în folderul **Calendar** .

5. Pentru a trimite un mesaj pentru a notifica delegatul pentru permisiunile modificate, bifați caseta de selectare se **trimite automat un mesaj către delegare rezumând aceste permisiuni** .
6. Dacă doriți, bifați caseta de selectare **delegatul poate vedea elementele mele private** .

    > [!IMPORTANT]
    > Această setare afectează toate folderele Exchange. Aceasta include toate folderele de corespondență, persoane de contact, calendar, activități, note și jurnal. Nu există nicio modalitate de a acorda acces la elemente personale doar în folderele specificate.

7. Alegeți **OK**.

    > [!NOTE]
    >
    > - Mesajele trimise cu permisiuni trimitere în numele includ atât delegatul, cât și numele de lângă **from**. Atunci când un mesaj este trimis cu permisiuni trimitere ca, se afișează doar numele dvs.
    > - După ce adăugați o persoană ca delegat, aceștia pot adăuga cutia poștală Exchange la profilul Outlook. Pentru instrucțiuni, consultați [gestionarea corespondenței și a elementelor de calendar ale altei persoane](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Pentru a elimina un delegat în Outlook pentru Windows:

1. Faceți clic pe fila **fișier** .
2. Faceți clic pe **Setări cont** , urmat de **delegare acces**.
3. Alegeți numele delegatului pentru care doriți să modificați permisiunile, apoi faceți clic pe **Eliminare** , urmat de **OK**.
