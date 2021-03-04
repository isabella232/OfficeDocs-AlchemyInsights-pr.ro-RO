---
title: Problemă cu un singur utilizator
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430204"
---
# <a name="problem-with-single-user"></a>Problemă cu un singur utilizator

- Este posibil ca utilizatorul să nu fi fost furnizat, deoarece serviciul nu a avut încă șansa de a evalua utilizatorul. Revizuiți instrucțiunile pentru durata de furnizare a accesului, precum și bara de progres de pe pagina de configurare a accesului. Dacă starea de echilibru specificată în secțiunea detalii suplimentare este înainte de data la care utilizatorul a fost creat/actualizat/șters, înseamnă că nu am evaluat încă utilizatorul. În acest scenariu, cel mai bun lucru de făcut este să așteptați ca serviciul de asigurare a accesului să se termine.

  - Rețineți că serviciul nostru cunoaște doar modificările aduse unui utilizator din sistemul sursă (Cloud HR). Trebuie să existe o modificare validă în sistemul sursă pentru Azure AD pentru a detecta modificarea și a o debita în Active Directory.
- Serviciul de asigurare a accesului a evaluat utilizatorul și a determinat că nu trebuie furnizat:
  - Dacă ați setat un filtru de definire bazat pe atribut, asigurați-vă că utilizatorul îndeplinește criteriile pe care le-ați specificat.
  - Dacă utilizatorii există deja în sistemul țintă și în starea utilizatorului în secțiunea sursă și țintă, nu vom mai întreprinde nicio acțiune suplimentară.
- Serviciul de asigurare a accesului a încercat să furnizeze utilizatorul și nu a reușit. Pentru aceste scenarii, examinați fila depanare și recomandări din jurnalele de asigurare a accesului:
  - Un atribut obligatoriu pentru utilizator poate fi lipsă în Active Directory local sau Azure AD. De exemplu, regulile de generare userPrincipalName sau sAMAccountName nu generează valoarea corectă.
  - Atributul corespondent (de obicei IDAngajat) nu se rezolvă cu un utilizator unic în Active Directory local sau Azure AD. De exemplu, există doi utilizatori cu aceeași IDAngajat în AD și serviciul returnează un cod de eroare indicând intrările țintă dublate pentru aceeași intrare sursă.

Pentru a revizui jurnalele pentru un singur utilizator și grupuri, consultați [revizuirea jurnalelor de asigurare a accesului pentru o problemă cu un anumit utilizator](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
