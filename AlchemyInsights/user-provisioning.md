---
title: Asigurarea accesului pentru utilizatori
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971351"
---
# <a name="user-provisioning"></a>Asigurarea accesului pentru utilizatori

- Utilizați capacitatea [de asigurare a accesului la cerere](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) pentru a asigurarea accesului unui utilizator și a obține diagnostice detaliate despre pașii urmați.
- Pentru a depana problemele pe care le întâmpinați atunci când asigurarea accesului pentru utilizatori și grupuri, consultați Ghidul de depanare [Nu se asigurarea accesului pentru utilizatori.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Dacă observați că nu se asigurarea accesului utilizatorilor, consultați Asigurarea accesului [cu jurnale (previzualizare)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) în Azure Active Directory (AD). Căutați intrări de jurnal care aparțin unui anumit utilizator.
- Reporniți periodic asigurarea accesului pentru a prinde toți utilizatorii care au fost omiți într-un ciclu anterior de asigurare a accesului.
- Este posibil ca utilizatorul/grupul să nu fi fost asigurat pentru că serviciul nostru nu a avut ocazia încă să evalueze utilizatorul. Revizuiți instrucțiunile pentru timpul de asigurare a accesului, precum și bara de progres de pe pagina de configurare a accesului. Dacă starea constantă specificată în secțiunea de detalii suplimentare este înainte de data la care utilizatorul a fost creat/actualizat/șters, înseamnă că nu am evaluat încă utilizatorul. În acest scenariu, cel mai bun lucru este să așteptați să se termine serviciul de asigurare a accesului. Dacă s-a atins starea constantă, vă recomandăm să efectuați o repornire din interfața de utilizator în portalul Azure.
  - Rețineți că serviciul nostru cunoaște doar modificările unui utilizator/grup din sistemul sursă (sistemul Azure Active Directory). Dacă un utilizator/un grup este eliminat direct din aplicație (de exemplu, ServiceNow), nu cunoaștem aceste modificări și nu le anulăm pe baza stării utilizatorului în sistemul sursă. În acest scenariu, cel mai bine este să reveniți la modificarea direct în aplicația țintă.
- Serviciul nostru a evaluat utilizatorul/grupul și a determinat că nu trebuie asigurată asigurarea accesului:
  - Dacă ați setat domeniul pentru utilizatorii și grupurile atribuite, verificați dacă s-a atribuit utilizatorul/grupul aplicației.
  - Dacă utilizatorului/grupului i se atribuie aplicația, asigurați-vă că nu i se atribuie rolul de acces implicit. Acest rol nu poate fi utilizat pentru asigurarea accesului.
  - Dacă ați setat un filtru de domeniu bazat pe atribut, asigurați-vă că utilizatorul îndeplinește criteriile pe care le-ați specificat.
  - Dacă utilizatorii există deja în sistemul țintă și starea utilizatorului în potrivirea sursă și țintă, nu vom mai lua nicio măsură suplimentară.
- Serviciul nostru a încercat să asigurarea accesului pentru utilizator și acesta a eșuat. Pentru aceste scenarii, revizuiți fila depanare și recomandări din jurnalele de asigurare a accesului:
  - Este posibil ca un atribut necesar pentru utilizator să lipsească Azure Active Directory sau să nu corespundă cu formatul solicitat de aplicația terță. De exemplu, atributul Country pentru un utilizator poate fi setat la Statele Unite, atunci când ar trebui să fie SUA.
  - Atributul este un atribut referențial care nu există încă în aplicația țintă. Un atribut referențial este un atribut care indică spre alt obiect, de exemplu, un utilizator care este membru al unui grup. ID-ul de utilizator ar fi în atributul membru al grupului, dar poate fi procesat doar dacă obiectul de utilizator la care indică există deja.
