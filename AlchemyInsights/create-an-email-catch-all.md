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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080758"
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
