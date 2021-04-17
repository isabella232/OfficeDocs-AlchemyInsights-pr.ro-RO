---
title: De ce este dezactivat butonul Adăugare buget pentru mine?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822647"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>De ce este dezactivat butonul Adăugare buget pentru mine?

Pentru a crea un buget, aveți nevoie de una dintre următoarele permisiuni:

- Management Group, Subscription, Resource Group Scopes
- Colaborator de gestionare a costurilor
- Proprietar
- Colaborator
- Doar clientul Enterprise: Înscriere, Departament, Domenii cont
- Administrator de înscriere (setați bugetul pentru domeniul de înscriere)
- Administrator de departament (setați bugetul în domeniul Departament)
- Proprietar cont (setați bugetul la domeniul de aplicare al contului)
- Doar acordul modern cu clientul: Contul de facturare, profilul de facturare, domeniile secțiunii Facturi
- Creator abonamente Azure

**Am creat un buget atunci când costul pentru luna curentă a fost deja supra-buget. De ce nu am primit o avertizare?**  
Dacă ați depășit deja un anumit prag de cost atunci când creați un buget, avertizarea respectivă nu va trage. După ce începe un nou ciclu, dacă încălcați pragul, avertizarea va fi trasă.

**Când ar trebui să mă aștept să primesc o avertizare după ce depășesc unul dintre pragurile de avertizare definite pentru buget?**  
Bugetele sunt evaluate la fiecare 4 ore. Durează minimum 8 ore pentru ca datele de utilizare să ajungă în sistemul de bugete. Cu această dată, avertizările pot dura nu mai mult de 12 ore pentru a fi trase după ce depășiți un prag.

**De ce este dezactivat butonul Data de început atunci când selectez o lună sau o perioadă de resetare a lunii de facturare?**  
Bugetele sunt aliniate la luna curentă din calendar sau la perioada de facturare curentă (în cazul în care este selectată Luna de facturare). Prin urmare, prepopulăm această valoare pentru tine.

**De ce nu văd un grafic cu costurile mele în experiența de creare a bugetului?**  
Avem nevoie de minimum 2 luni de date de cost înainte de a putea reda un grafic pentru a vă asista la crearea bugetului.

**De ce nu pot seta un buget pentru un abonament pe care tocmai l-am creat?**  
După crearea unui abonament, procesarea datelor durează 24-48 de ore înainte de stabilirea unui buget.

**Resurse API bugetat**

- [Budgets API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Provides operations to create and update budgets. Utilizând API-ul de bugete, puteți să setați un prag de buget și să configurați mai multe avertizări la fire pe măsură ce vă apropiați de pragul respectiv. Avertizările pot declanșa un mesaj de e-mail sau un grup de acțiune Azure pentru a efectua automatizarea. Notă: Filtrarea pentru acest API nu se aliniază cu filtrarea/dimensiunile API de interogare.
- [Budgets API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Create budgets with greater cost filtering capabilities than v1. Filtrarea se aliniază la contractul utilizat în API-urile pentru interogări și dimensiuni. Aceasta este API-ul de bugete recomandat pentru avansare.
- [Dimensiuni:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Furnizează operațiuni pentru a obține dimensiuni acceptate pentru utilizarea dvs. într-o varietate de domenii. Utilizând API-ul de dimensiuni, puteți regăsi o listă de dimensiuni care pot fi utilizate ca intrări pentru generarea interogărilor cu API-ul de interogare.
- [Interogare:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Furnizează operațiuni pentru a obține date de cost agregat și utilizare pe baza interogării pe care o furnizați. Utilizând API-ul de interogare, puteți specifica filtrele, sortarea și gruparea dorite după toate dimensiunile disponibile (care sunt accesate din API-ul de dimensiuni).

**Costuri prognozate**

**De ce nu văd prognozele pentru costurile mele în Analiza costurilor?**  
Există mai multe motive pentru care proiecția prognozare poate lipsi din analiza costurilor, unele dintre ele sunt după cum urmează:

1. Dacă datele despre cost sunt mai mici de 10 zile, diagrama prognoză nu se va încărca. Modelul necesită cel puțin 10 zile de date recente de cost pentru proiecții precise
2. Dacă ați selectat date istorice, diagrama de prognoză nu va fi vizibilă. Selectați un interval de date cu date viitoare pentru a se afișa diagrama de prognoză
3. În cazul în care contul dvs. are mai multe monede, diagrama de prognoză va include doar costurile proiectului pentru "Toate costurile în USD"

**De ce nu se modifică prognoza atunci când fac modificări la resursele mele?**  
Modelul de prognoză necesită câteva zile pentru a ține seama de modificările din cont și nu face proiecții imediate pe baza modificărilor din resurse  
Pentru pași mai mari de creștere sau descreștere a resurselor, ajustarea acestor modificări la resursele modelului va dura puțin mai mult

**De ce crește prognoza după ce fac o rezervare sau o achiziție de la Marketplace?**  
Modelul de prognoză ia în considerare "Cost real" și nu ține cont de utilizare și de achiziție separat. Pentru o achiziție cu o singură dată, modelul va micșora proiecțiile după 10 zile pentru a ține cont de creșterea dintr-o dată a costurilor

**Doresc să văd prognoze pentru o singură dimensiune (de exemplu, Metru)**  
Prognozarea acceptă în prezent proiecții totale de cost, nu pentru metri individuali. Astfel, atunci când "Grupat după" o dimensiune, proiecțiile se vor proiecta în total din toate elementele de dimensiune

**Documente recomandate**

- [Ce este Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Practici recomandate pentru Gestionarea costurilor Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizați costurile și cheltuielile](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorarea și analizarea costurilor cu analiza costurilor](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Prețuri](https://azure.microsoft.com/services/cost-management/#pricing)
- [Revizuirea costurilor în analiza costurilor](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial video: Crearea unui buget în portalul Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Cerințe preliminare pentru vizualizarea și particularizarea bugetelor](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Crearea și gestionarea bugetelor](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurarea automatizarei cu API-ul Grupuri de acțiuni Azure și Bugete](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Utilizarea avertizărilor de cost pentru monitorizarea utilizării și cheltuielilor](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Practici recomandate pentru gestionarea costurilor](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Tutoriale video**

- [Crearea unui buget în portalul Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gestionarea costurilor cu API-ul de bugete și grupurile de acțiuni](https://go.microsoft.com/fwlink/?linkid=2147038)