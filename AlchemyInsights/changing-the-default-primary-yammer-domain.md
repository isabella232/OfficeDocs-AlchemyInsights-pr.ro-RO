---
title: Schimbarea domeniului Yammer implicit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817996"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Schimbarea domeniului Yammer implicit/principal

Adresa URL Yammer conține numele de domeniu principal curent pentru rețeaua dvs. Yammer. Acest nume de domeniu poate să nu corespundă cu numele principal de domeniu setat în Office 365 sau Azure AD. Există diferențe de comportament pe baza numărului de domenii particularizate adăugate entității găzduite și dacă Yammer se află sau nu într-o configurație acceptată (1 entitate găzduită: 1 rețea sau 1:1). Este disponibilă documentația despre [domeniile Yammer și Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Motivul cel mai obișnuit pentru care vedeți un domeniu incorect este că există mai multe rețele Yammer și trebuie să fie unificate. [Unificarea la o singură rețea](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) utilizând instrumentul de migrare în rețea reprezintă un prim pas important. Finalizați acest lucru înainte de a încerca să setați domeniul principal.

**Nu există domenii particularizate**

Pentru entitățile găzduite noi, domeniul implicit (de exemplu, fabrikam.onmicrosoft.com) din entitatea găzduită va fi utilizat pentru Yammer. Domeniul principal este setat la yammer.com/fabrikam.onmicrosoft.com.

**Un singur domeniu particularizat**

Yammer va selecta automat domeniul particularizat (de exemplu, fabrikam.com) din entitatea găzduită drept domeniu principal în Yammer. Acesta este setat la yammer.com/fabrikam.com. Această modificare se face de către serviciul de sincronizare a domeniului și poate necesita până la 24 de ore pentru a se aplica.

**Mai multe domenii particularizate**

Yammer poate avea un domeniu principal diferit de domeniul entității găzduite implicite. Deoarece există mai multe domenii particularizate, Yammer nu încearcă să ghicească domeniul corect din cele disponibile. Trebuie să deschideți un caz de asistență pentru a solicita ca numele de domeniu principal să fie schimbat în domeniul principal pe care îl alegeți.

**Informații suplimentare despre depanare**

În unele cazuri, este posibil ca anumite domenii să fi fost mutate între entitățile găzduite și serviciul de sincronizare a domeniului nu a reușit să ruleze cu succes. Este posibil să vă confruntați cu probleme de conectare sau cu alte probleme, pe lângă problema cu domeniul principal incorect. Pentru a rezolva această problemă, ar putea fi necesar ca domeniile să fie mutate în rețeaua corectă, cu ajutorul Asistenței Microsoft. Această situație necesită asistență directă și rezolvarea poate dura ceva timp, mai ales dacă există o listă foarte lungă de nume de domenii. Deschideți un caz de asistență pentru a obține ajutor cu rezolvarea acestor tipuri de probleme.

Atunci când lucrați cu un agent de asistență, aceștia vor verifica dacă domeniile sunt verificate pe o entitate găzduită sub controlul dvs. Aceștia pot pune întrebări de verificare suplimentare despre domeniile dvs. dacă sunt adăugate la entitatea găzduită, dar nu sunt verificate prin DNS. Asigurați-vă că domeniile sunt verificate prin DNS pentru a accelera procesul.
