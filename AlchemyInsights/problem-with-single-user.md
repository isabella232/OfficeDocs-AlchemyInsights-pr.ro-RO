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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960163"
---
# <a name="problem-with-single-user"></a>Problemă cu un singur utilizator

- Este posibil ca utilizatorul să nu fi avut acces asigurat deoarece serviciul nu a avut ocazia încă să evalueze utilizatorul. Revizuiți instrucțiunile pentru timpul de asigurare a accesului, precum și bara de progres de pe pagina de configurare a accesului. Dacă starea constantă specificată în secțiunea de detalii suplimentare este înainte de data la care utilizatorul a fost creat/actualizat/șters, înseamnă că nu am evaluat încă utilizatorul. În acest scenariu, cel mai bun lucru este să așteptați să se termine serviciul de asigurare a accesului.

  - Rețineți că serviciul nostru cunoaște numai modificările aduse unui utilizator în sistemul sursă (Resurse umane în cloud). Trebuie să existe o modificare validă în sistemul sursă pentru Azure AD pentru a detecta modificarea și a o fluxul în Active Directory.
- Serviciul de asigurare a accesului a evaluat utilizatorul și a determinat că nu trebuie asigurat acest lucru:
  - Dacă ați setat un filtru de domeniu bazat pe atribut, asigurați-vă că utilizatorul îndeplinește criteriile pe care le-ați specificat.
  - Dacă utilizatorii există deja în sistemul țintă și starea utilizatorului în potrivirea sursă și țintă, nu vom mai lua nicio măsură suplimentară.
- Serviciul de asigurare a accesului a încercat să asigurarea accesului pentru utilizator și acesta a eșuat. Pentru aceste scenarii, revizuiți fila depanare și recomandări din jurnalele de asigurare a accesului:
  - Este posibil ca atributul necesar al utilizatorului să lipsească în Active Directory local sau Azure AD. De exemplu, regulile de generare a regulilor userPrincipalName sau sAMAccountName nu generează valoarea corectă.
  - Atributul potrivit (de obicei id angajat) nu se rezolvă pentru un utilizator unic din Active Directory local sau Azure AD. De exemplu, există doi utilizatori cu acelașiid angajat în AD, iar serviciul returnează un cod de eroare care indică intrările țintă dublate pentru aceeași intrare sursă.

Pentru a examina jurnalele pentru un singur utilizator și grupuri, consultați [Examinarea jurnalelor de asigurare a accesului pentru o problemă cu un anumit utilizator.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
