---
title: De ce butonul Adăugare buget este dezactivat pentru mine?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807667"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>De ce butonul Adăugare buget este dezactivat pentru mine?

Pentru a crea un buget, aveți nevoie de una dintre următoarele permisiuni:

- Grup de gestionare, abonament, domenii de grup de resurse
- Contribuitor la gestionarea costurilor
- Proprietar
- Contribuitor
- Numai pentru clienți de întreprindere: înscriere, departament, domenii de cont
- Administrator de înscriere (setați bugetul la domeniul de înscriere)
- Administrator de departament (setați bugetul la domeniul departamentului)
- Proprietar cont (setați bugetul la domeniul de cont)
- Numai acordul clienți modern: cont de facturare, profil de facturare, domenii de secțiune a facturii
- Creator abonament Azure

**Am creat un buget atunci când costurile pentru luna curentă erau deja supra-bugetare. De ce nu am primit o avertizare?**  
Dacă ați depășit deja un prag de cost dat atunci când creați un buget, avertizarea nu va fi trasă. După ce începe un nou ciclu, dacă încălcați pragul, avertizarea va fi trasă.

**Când ar trebui să mă aștept să primesc o avertizare după ce depășesc unul dintre pragurile de avertizare bugetare definite?**  
Bugetele sunt evaluate la fiecare 4 ore. Este nevoie de minimum 8 ore pentru ca datele de utilizare să ajungă la sistemul de bugete. Ținând cont de aceasta, avertizările pot dura până la 12 ore până când depășiți un prag.

**De ce butonul dată de început este dezactivat atunci când selectez o perioadă de resetare lunară sau de facturare?**  
Bugetele sunt aliniate la luna curentă a calendarului sau la perioada de facturare curentă (în cazul în care este selectată luna de facturare). Prin urmare, vom pre-popula această valoare pentru dvs.

**De ce nu văd un grafic al costurilor mele în experiența de creare a bugetului?**  
Avem nevoie de minim 2 luni de date de cost înainte de a putea reda un grafic pentru a vă ajuta cu crearea bugetului.

**De ce nu pot seta un buget pentru un abonament pe care tocmai l-am creat?**  
După crearea unui abonament, datele durează 24-48 de ore pentru a procesa înainte de a stabili un buget împotriva acestuia.

**Resurse API bugetare**

- [API-bugete v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): furnizează operațiuni pentru a crea și a actualiza bugetele. Utilizând API-ul bugete, puteți să setați un prag bugetar și să configurați mai multe avertizări la foc în timp ce vă apropiați de acel prag. Avertizările pot declanșa un mesaj de e-mail sau un grup de acțiuni Azure pentru a efectua automatizare. Notă: filtrarea pentru acest API nu se aliniază cu filtrarea/dimensiunile API-ului de interogare.
- [Bugete API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Creați bugete cu capacități mai mari de filtrare a costurilor decât v1. Filtrarea se aliniază la contractul utilizat în API-urile noastre de interogare și dimensiuni. Acesta este API-ul bugetelor recomandate pentru a utiliza Mutarea înainte.
- [Dimensiuni](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): furnizează operații pentru a obține dimensiuni acceptate pentru utilizare sub o varietate de domenii. Utilizând API-ul de dimensiuni, puteți regăsi o listă de dimensiuni care pot fi utilizate ca intrări pentru generarea interogărilor cu API-ul de interogare.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): furnizează operații pentru a obține date despre costurile agregate și utilizare pe baza interogării pe care o furnizați. Utilizând API-ul de interogare, puteți specifica filtrarea dorită, sortarea și gruparea la toate dimensiunile disponibile (care sunt accesate din API-ul de dimensiuni).

**Costuri prognozate**

**De ce nu văd prognoze pentru costurile mele în analiza costurilor?**  
Există mai multe motive pentru care este posibil ca proiecția Prognoză să lipsească în analiza costurilor, unele dintre ele sunt după cum urmează:

1. Dacă datele de cost sunt mai vechi de 10 zile, diagrama Prognoză nu se va încărca. Modelul necesită cel puțin 10 zile de date de cost recente pentru proiecții precise
2. Dacă ați selectat date istorice, atunci diagrama Prognoză nu va fi vizibilă. Vă rugăm să selectați un interval de date cu datele viitoare pentru ca diagrama Prognoză să fie afișată
3. Dacă aveți mai multe monede în cont, diagrama Prognoză va costa doar costurile pentru "toate costurile în USD"

**De ce nu se modifică Prognoza atunci când fac modificări la resursele mele?**  
Modelul de Prognoză necesită câteva zile pentru a lua în considerare modificările din cont și nu face proiecții imediate pe baza modificărilor resurselor  
Pentru pași mai mari de mărire sau micșorare a resurselor, modelul va dura mai mult timp pentru a ajusta aceste modificări în funcție de anomalii

**De ce crește Prognoza mea după ce fac o rezervare sau o achiziție pe piață?**  
Modelul de Prognoză consideră "costul real" și nu răspunde pentru utilizare și cumpărare separat. Pentru o achiziție unică, modelul va scădea proeminențele după 10 zile pentru a ține cont de creșterea bruscă a costurilor

**Doresc să văd prognoze pentru o singură dimensiune (de exemplu,. Contorului**  
Prognoza acceptă în prezent proiecții totale ale costului, nu pentru contoare individuale. Prin urmare, când "grupat după" o dimensiune, proiecțiile vor fi pentru totalul tuturor elementelor din dimensiune

**Documente recomandate**

- [Ce este managementul costurilor Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cele mai bune practici de gestionare a costurilor Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizarea costurilor și cheltuielilor](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorarea și analizarea costurilor cu analiza costurilor](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gestionarea costurilor Azure: prețuri](https://azure.microsoft.com/services/cost-management/#pricing)
- [Revizuirea costurilor din analiza costurilor](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial video: crearea unui buget în portalul Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Cerințe preliminare pentru vizualizarea și particularizarea bugetelor](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Crearea și gestionarea bugetelor](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurarea automatizarii cu Azure Action Groups și budgets API](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Utilizarea avertizărilor de cost pentru a monitoriza utilizarea și cheltuielile](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cele mai bune practici de gestionare a costurilor](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Videoclipuri tutorial**

- [Crearea unui buget în portalul Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gestionarea costurilor cu API-ul bugetele și grupurile de acțiuni](https://go.microsoft.com/fwlink/?linkid=2147038)