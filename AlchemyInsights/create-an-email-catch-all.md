---
title: Creați un mesaj de e-mail pentru a vă prinde tot
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816212"
---
# <a name="create-an-email-catch-all"></a>Creați un mesaj de e-mail pentru a vă prinde tot

Utilizarea unei capturi este foarte puternică. Este mai bine să furnizați expeditorului o returnată, prin care expeditorii să știe că mesajul lor nu poate fi livrat ca adresat, astfel încât să poată lua măsuri. De asemenea, puteți limita cutia poștală monitorizată pentru a captura doar adresele de e-mail valide anterior. 

Orice cutie poștală de tip catch will receive a good deal of spam (Spam) și poate completa în cele din urmă dacă nu este monitorizată îndeaproape. (Există limite pentru primirea de date.) 

Dacă decideți să continuați, urmați acești pași:

1. Crearea unui grup de distribuire dinamic include & "Toate tipurile de destinatari".

2. Creați o cutie poștală dedicată pentru a vă prinde mesajele de e-mail, de exemplu, catchall@domain.com.

3. Pentru domeniul specific, setați DomainType la "InternalRelay". Dacă mai târziu eliminați toate capturile, asigurați-vă că setați domeniul înapoi la Autoritate.

4. Creați o regulă de transport de flux de corespondență după cum urmează:

    - Dacă expeditorul este "în afara organizației"
    - Redirijați mesajul către Catchall@domain.com
    - Cu excepția cazului în care destinatarul este membru allusers@domain.com (Grupul de distribuire conține toți membrii)
    - Asigurați-vă că validați faptul că noile cutii poștale sunt adăugate la grupul de distribuire dinamic
