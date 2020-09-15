---
title: Crearea unui mesaj de e-mail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712998"
---
# <a name="create-an-email-catch-all"></a>Crearea unui mesaj de e-mail

Utilizarea unei captură toate este puternic descurajată. Este mai bine să oferiți o revenire la expeditor, permițându-le expeditorilor să știe că mesajul său nu a putut fi livrat așa cum este adresat, astfel încât aceștia să poată lua măsuri. De asemenea, puteți limita cutia poștală monitorizată pentru a prinde doar adresele de e-mail valide anterior. 

Orice captură a cutiei poștale va primi o bună cantitate de spam și se poate umple în cele din urmă dacă nu este monitorizată îndeaproape. (Există limite de primire.) 

Dacă decideți să continuați, urmați acești pași:

1. Creați un grup de distribuire dinamic & includeți "toate tipurile de destinatari".

2. Creați o cutie poștală dedicată pentru a prinde mesaje de e-mail, de exemplu, catchall@domain.com.

3. Pentru domeniul specific, setați DomainType la "InternalRelay". Dacă mai târziu eliminați toate captură, asigurați-vă că setați domeniul înapoi la autoritate.

4. Creați o regulă de transport fluxul după cum urmează:

    - Dacă expeditorul este "în afara organizației"
    - Redirecționați mesajul către Catchall@domain.com
    - Cu excepția cazului în care destinatarul este membru al allusers@domain.com (grupul de distribuire conține toți membrii)
    - Asigurați-vă că validați noile cutii poștale sunt adăugate în grupul de distribuire dinamic
