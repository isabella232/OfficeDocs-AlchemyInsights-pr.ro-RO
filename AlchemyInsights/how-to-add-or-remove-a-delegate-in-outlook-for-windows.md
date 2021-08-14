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
ms.openlocfilehash: ee54e2bcca4f4591b33ee805290192311f6cde09a9e453a813e9db328d19634d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945349"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Cum se adaugă sau se elimină un delegat în Outlook pentru Windows

Pentru a adăuga un delegat în Outlook pentru Windows: 

1. Faceți clic **pe fila** Fișier, urmat **de Setări**, apoi alegeți **Delegare acces.**
2. Faceți clic **pe Adăugare.** Dacă **nu** apare Adăugare, este posibil să nu existe o conexiune activă între Outlook și Exchange. Bara Outlook de stare afișează starea conexiunii.
3. Tastați numele persoanei pe care doriți să o desemnați ca delegatul dvs. sau căutați-o și alegeți numele în lista de rezultate de căutare.

    > [!NOTE]
    > Delegatul trebuie să fie o persoană din lista globală de adrese Exchange (GAL) a organizației dvs.
4. Faceți clic **pe Adăugare,** urmat de **OK.**
5. În caseta de dialog **Delegare** permisiuni, acceptați setările de permisiune implicite sau selectați niveluri de acces particularizate Exchange folderele.

    - Dacă un delegat are nevoie de permisiuni pentru a lucra numai  cu solicitări de întâlniri și răspunsuri, sunt suficiente setările de permisiuni implicite, cum ar fi Delegatul primește copii ale mesajelor legate de întâlnirile personale. Setarea de permisiune pentru **Inbox poate** fi lăsată la **Fără.** Solicitările de întâlnire și răspunsurile vor fi primite direct în inboxul delegatului.

    > [!NOTE]
    > Implicit, delegatului i se acordă **permisiunea Editor (citește, creează și modifică elemente)** în **folderul Calendar.** Atunci când delegatul răspunde la o întâlnire în numele dvs., aceasta se adaugă automat la **folderul** Calendar.

5. Pentru a trimite un mesaj care să anunțe delegatul despre permisiunile modificate, bifați caseta de selectare Trimiteți automat un mesaj **delegatului,** care să rezume aceste permisiuni.
6. Dacă doriți, bifați caseta **de selectare Posibilitatea ca delegatul să vadă elementele** personale.

    > [!IMPORTANT]
    > Această setare afectează toate Exchange foldere. Între acestea se numără toate folderele Corespondență, Persoane de contact, Calendar, Activități, Note și Jurnal. Nu există nicio modalitate de a acorda acces la elementele personale doar pentru folderele specificate.

7. Alegeți **OK.**

    > [!NOTE]
    >
    > - Mesajele trimise cu permisiuni Trimitere în numele includ atât numele delegatului, cât și al dvs. lângă De **la**. Atunci când se trimite un mesaj cu permisiuni Trimitere ca, apare doar numele dvs.
    > - După ce adăugați pe cineva ca delegat, persoana vă poate adăuga cutia Exchange poștală la Outlook dvs. de e-mail. Pentru instrucțiuni, consultați Gestionarea [corespondenței și a elementelor de calendar ale altei persoane.](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)

Pentru a elimina un delegat din Outlook timp Windows:

1. Faceți clic **pe fila** Fișier.
2. Faceți clic **pe Setări** de cont, urmat **de Delegare acces.**
3. Alegeți numele delegatului pentru care doriți să modificați permisiunile, apoi faceți clic pe **Eliminare urmat** de **OK.**
