---
title: Creați o captură prin e-mail pe toate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286204"
---
# <a name="create-an-email-catch-all"></a>Creați o captură prin e-mail pe toate

Utilizarea unei capturi toate este puternic descurajat. Este mai bine pentru a oferi o saritura înapoi la expeditor închirierea expeditorilor știu mesajul lor nu a putut fi livrate ca abordate, astfel încât acestea să poată lua măsuri. De asemenea, puteți limita cutia poștală monitorizată pentru a prinde numai adresele de e-mail valide anterior. 

Orice captură toate cutia poștală va primi o afacere bună de spam și poate umple în cele din urmă, dacă nu monitorizate îndeaproape. (Există limite de primire.) 

Dacă decideți să continuați, urmați acești pași:

1. Creați un grup de distribuire dinamic & include "Toate tipurile de destinatari".

2. Creați o cutie poștală dedicată pentru a prinde e-mailuri, de exemplu, catchall@domain.com.

3. Pentru domeniul specific, setați DomainType la "InternalRelay". Dacă mai târziu eliminați captura toate, asigurați-vă că pentru a seta domeniul înapoi la cu autoritate.

4. Creați o regulă de transport mailflow după urmează:

    - Dacă Expeditorul este "În afara organizației"
    - Redirecționați mesajul către Catchall@domain.com
    - Cu excepția cazului în care destinatarul este membru al allusers@domain.com (Grupul de distribuire conține toți membrii)
    - Asigurați-vă că pentru a valida că noile cutii poștale sunt adăugate în grupul de distribuire dinamică
