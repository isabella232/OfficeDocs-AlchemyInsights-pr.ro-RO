---
title: Probleme de autentificare
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974794"
---
# <a name="authentication-issues"></a>Probleme de autentificare

**Căutați informații despre codurile de eroare AADSTS care sunt returnate din serviciul token de securitate Azure Active Directory (Azure AD)?** Consultați [codurile de eroare pentru autentificarea și autorizarea AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pentru a găsi descrieri de erori AADSTS, remedieri și câteva soluții sugerate.

Erorile de autorizare pot fi rezultatul mai multor probleme diferite, majoritatea generând o eroare 401 sau 403. De exemplu, următoarele probleme pot duce la erori de autorizare:

- [Fluxuri de achiziție token Access](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorecte 
- [Domenii de permisiune](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) configurate slab 
- Lipsă de [consimțământ](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Pentru a rezolva erorile comune de autorizare, încercați pașii furnizați mai jos, care se potrivește cel mai bine cu eroarea pe care o primiți. Se pot aplica mai mult de un pas pentru o eroare pe care o primiți.

- **eroare neautorizată 401: simbolul este valid?**

Asigurați-vă că aplicația prezintă un token de acces valid la Microsoft Graph ca parte a solicitării. Această eroare înseamnă adesea că simbolul de acces poate să lipsească din antetul de solicitare de autentificare HTTP sau că simbolul nu este valid sau a expirat. Vă recomandăm insistent să utilizați biblioteca de autentificare Microsoft (MSAL) pentru achiziționarea de simboluri Access. În plus, această eroare poate apărea dacă încercați să utilizați un simbol de acces delegat acordat unui cont Microsoft personal pentru a accesa un API care acceptă doar conturile de la locul de muncă sau de la școală (conturi organizaționale).

**eroare interzisă 403: ați ales setul corect de permisiuni?**

Asigurați-vă că ați solicitat setul corect de permisiuni pe baza API-urilor Microsoft Graph efectuate de aplicații. Permisiunile recomandate cel mai puțin privilegiat sunt furnizate în toate subiectele metodei de referință Microsoft Graph API. În plus, aceste permisiuni trebuie să fie acordate aplicației de către un utilizator sau de către un administrator. Acordarea permisiunilor se întâmplă în mod normal printr-o pagină de consimțământ sau utilizarea lamei de înregistrare a aplicației Azure portal. Din lama de **Setări** pentru aplicație, faceți clic pe **permisiuni necesare**, apoi faceți clic pe **acordare permisiuni**. Pentru mai multe informații, consultați:

- [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Înțelegerea permisiunilor și consimțământului Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**eroare interzisă 403: aplicația a obținut un token pentru a se potrivi cu permisiunile alese?**

Asigurați-vă că tipurile de permisiuni solicitate sau acordate corespund tipului de token de acces pe care îl dobândește aplicația dvs. Este posibil să solicitați și să acordați permisiuni de aplicație, dar să utilizați tokenuri de flux de cod interactiv delegat în locul tokenurilor flux de acreditare client sau să solicitați și să acordați permisiuni delegate, dar să utilizați tokenuri de flux de acreditare client în locul tokenurilor flux de cod delegate.

Pentru mai multe informații legate de achiziționarea tokenurilor, consultați:

- [Obțineți acces în numele utilizatorilor și al permisiunilor delegate](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 codul de autorizare flux](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obțineți acces fără un utilizator (Serviciu Daemon) și permisiuni de aplicație](https://docs.microsoft.com/graph/auth-v2-service) 
- [Flux de acreditări client Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**eroarea interzisă 403: Reinițializarea parolei**

În prezent, nu există permisiuni de aplicație daemon service-to-service care permit reinițializarea parolelor utilizatorilor. Aceste API-uri sunt acceptate doar utilizând fluxurile de coduri interactive delegate cu un administrator conectat. Pentru mai multe informații, consultați [permisiunile Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 interzis: utilizatorul are acces și este licențiat?**

Pentru fluxurile de coduri delegate, Microsoft Graph evaluează dacă solicitarea a fost permisă în funcție de permisiunile acordate aplicației și de permisiunile pe care le are utilizatorul conectat. În general, această eroare indică faptul că utilizatorul nu este suficient de privilegiat pentru a efectua solicitarea **sau** că utilizatorul nu are licență pentru datele care se accesează. Numai utilizatorii cu permisiuni sau licențe necesare pot face solicitarea cu succes.

**403 interzis: ați selectat API-ul de resurse corect?**

Servicii API precum Microsoft Graph Verificați dacă afirmația *aud* (audiența) din simbolul Access primit se potrivește cu valoarea pe care o așteaptă de la sine și, dacă nu, apare o eroare de 403 interzisă. O greșeală comună care rezultă din această eroare încearcă să utilizeze un token dobândit pentru API-uri Azure AD Graph, API-uri Outlook sau SharePoint/OneDrive pentru a apela Microsoft Graph (sau invers). Asigurați-vă că resursa (sau domeniul de aplicare) aplicația achiziționează un token pentru potrivește cu API-ul pe care îl solicită aplicația.

**400 Solicitare eronată sau 403 interzisă: utilizatorul respectă politicile de acces condiționat (CA) ale Organizației?**

Pe baza politicilor de acces condiționat (CA) ale unei organizații, un utilizator care accesează resurse Microsoft Graph prin intermediul aplicației poate fi contestat pentru informații suplimentare care nu sunt prezente în tokenul Access pe care l-a achiziționat inițial aplicația. În acest caz, aplicația primește un **400 cu** o eroare de interaction_required în timpul achiziționării tokenului de acces sau al unui **403 cu eroarea *Insufficient_claims*** atunci când se solicită Microsoft Graph. În ambele cazuri, răspunsul de eroare conține informații suplimentare care pot fi prezentate punctului final autorizat pentru a-i provoca utilizatorului informații suplimentare (cum ar fi autentificarea cu mai mulți factori sau înscrierea dispozitivelor).

Pentru mai multe informații despre accesul condiționat, consultați:

- [Gestionarea provocărilor accesului condiționat utilizând MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Ghid pentru dezvoltatori pentru acces condițional Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica) și AZURE AD Graph API (AAD Graph)_* _

- Începând cu 30 iunie, 2020, nu vom mai adăuga caracteristici noi la Azure Active Directory Authentication Library (monica) și Azure AD Graph API (AAD Graph). Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.
- Începând cu 30 iunie, 2022, vom încheia suportul pentru monica și Dan grafic și nu va mai furniza asistență tehnică sau actualizări de securitate.
    - Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi nicio asistență tehnică sau actualizări de securitate.
    - Este posibil ca aplicațiile care utilizează Dan Graph să nu mai primească răspunsuri de la punctul final din punct grafic.

-*Migrarea* monica*

Vă recomandăm să actualizați la [biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate. Această recomandare se află în contextul în care Microsoft își migrează aplicațiile către MSAL până la termenul limită de finalizare a asistenței. Obiectivul migrării Microsoft Apps la MSAL este acela de a vă asigura că aplicațiile beneficiază de îmbunătățiri ale securității și caracteristicii MSAL în curs de desfășurare.

- [Citiți întrebări frecvente despre Monica](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Aflați cum să migrați aplicațiile pe o bază per platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Dacă aveți nevoie de ajutor pentru a înțelege care dintre aplicațiile dumneavoastră utilizează Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați vânzătorii de software independenți (ISV) sau furnizorii de aplicații. Asistența Microsoft vă poate oferi, de asemenea, o listă cu toate aplicațiile non-Microsoft Monica din entitatea găzduită.

**Migrarea graficului AAD**

Pentru aplicațiile care utilizează AAD Graph, urmați ghidul nostru pentru a [migra aplicațiile AZURE AD Graph la Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Lista de verificare a migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portalul de înregistrare Azure App Arată ce aplicații utilizează Dan Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor și, dacă este cazul, să contactați orice ISV sau furnizori de aplicații. Asistența Microsoft vă poate oferi, de asemenea, informații despre utilizarea tuturor grafurilor în entitatea găzduită.

 










