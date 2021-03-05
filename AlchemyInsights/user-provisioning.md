---
title: Asigurarea accesului utilizatorilor
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
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482918"
---
# <a name="user-provisioning"></a>Asigurarea accesului utilizatorilor

- Utilizați capacitatea de furnizare la [cerere](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) pentru a asigura un utilizator și a obține diagnostice detaliate despre pașii luați.
- Pentru a depana problemele pe care le întâmpinați atunci când furnizați utilizatori și grupuri, consultați Ghidul de depanare [niciun utilizator nu este furnizat](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Dacă observați că nu este furnizat utilizatorilor, consultați [jurnale de asigurare a accesului (Previzualizare)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) în Azure Active Directory (AD). Căutați intrări în jurnal legate de un anumit utilizator.
- Reporniți periodic asigurarea accesului pentru a prinde toți utilizatorii care au fost omiteți într-un ciclu de asigurare a accesului anterior.
- Este posibil ca utilizatorul/grupul să nu fi fost furnizat, deoarece serviciul nostru nu a avut încă șansa de a evalua utilizatorul. Revizuiți instrucțiunile pentru durata de furnizare a accesului, precum și bara de progres de pe pagina de configurare a accesului. Dacă starea de echilibru specificată în secțiunea detalii suplimentare este înainte de data la care utilizatorul a fost creat/actualizat/șters, înseamnă că nu am evaluat încă utilizatorul. În acest scenariu, cel mai bun lucru de făcut este să așteptați ca serviciul de asigurare a accesului să se termine. Dacă starea de echilibru a fost realizată, vă recomandăm să efectuați o repornire din interfața de utilizator din portalul Azure.
  - Rețineți că serviciul nostru este conștient doar de modificările aduse unui utilizator/grup din sistemul sursă (Azure Active Directory). Dacă un utilizator/grup este eliminat direct din aplicație (de exemplu, ServiceNow), nu suntem conștienți de aceste modificări și nu îl returnăm în funcție de starea utilizatorului din sistemul sursă. În acest scenariu, cel mai bine este să reveniți la modificarea direct în aplicația țintă.
- Serviciul nostru a evaluat utilizatorul/grupul și a determinat că nu trebuie furnizat:
  - Dacă ați setat domeniul pentru utilizatori și grupuri atribuite, Verificați dacă utilizatorul/grupul este atribuit aplicației.
  - Dacă utilizatorul/grupul este atribuit aplicației, asigurați-vă că nu i se atribuie rolul de acces implicit. Acest rol nu poate fi utilizat pentru asigurarea accesului.
  - Dacă ați setat un filtru de definire bazat pe atribut, asigurați-vă că utilizatorul îndeplinește criteriile pe care le-ați specificat.
  - Dacă utilizatorii există deja în sistemul țintă și în starea utilizatorului în secțiunea sursă și țintă, nu vom mai întreprinde nicio acțiune suplimentară.
- Serviciul nostru a încercat să furnizeze utilizatorul și nu a reușit. Pentru aceste scenarii, examinați fila depanare și recomandări din jurnalele de asigurare a accesului:
  - Un atribut obligatoriu pentru utilizator poate lipsi din Azure Active Directory sau nu se potrivește cu formatul necesar pentru aplicația terță parte. De exemplu, atributul țară pentru un utilizator poate fi setat la Statele Unite atunci când ar trebui să fie noi.
  - Atributul este un atribut Referențial care nu există încă în aplicația țintă. Un atribut Referențial este un atribut care indică spre alt obiect, de exemplu, un utilizator care este membru al unui grup. ID-ul utilizatorului ar fi în atributul membru al grupului, dar poate fi procesat doar dacă obiectul de utilizator indică existența deja.
