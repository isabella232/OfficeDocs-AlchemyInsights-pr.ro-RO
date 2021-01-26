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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976861"
---
# <a name="authentication-issues"></a>Probleme de autentificare

**Căutați informații despre codurile de eroare AADSTS returnate de la serviciul toekn de securitate (STS) Azure Active Directory (Azure AD)?** Consultați [Coduri de eroare de autentificare și autorizare Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pentru a găsi descrieri ale erorilor AADSTS, remedieri și unele soluții sugerate.

Erorile de autorizare pot rezulta din mai multe probleme diferite, majoritatea generând o eroare 401 sau 403. De exemplu, următoarele probleme pot duce la erori de autorizare:

- [Fluxuri de acces](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) incorecte 
- [Domenii de permisiune](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) incorect configurate 
- Lipsa [consimțământului](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Pentru a rezolva erorile comune de autorizare, încercați pașii de mai jos care se potrivesc cel mai bine cu eroarea pe care o primiți. Este posibil să se aplice mai mulți pași pentru o eroare pe care o primiți.

**Eroare 401 Neautorizat: Tokenul dvs. este valid?**

Asigurați-vă că aplicația dvs. prezintă un token de acces valid la Microsoft Graph ca parte a solicitării. Această eroare înseamnă adesea că tokenul de acces poate lipsi din antetul solicitării HTTP de autentificare sau că tokenul nu este valid sau a expirat. Vă recomandăm ferm să utilizați Biblioteca de autentificare Microsoft (MSAL) pentru achiziționarea tokenurilor de acces. În plus, această eroare poate apărea dacă încercați să utilizați un token de acces delegat acordat unui cont Microsoft personal pentru a accesa un API care acceptă doar conturi de la locul de muncă sau de la școală (conturi de organizație).

**Eroare 403 Interzis: Ați ales setul corect de permisiuni?**

Asigurați-vă că ați solicitat setul corect de permisiuni pe baza API-urilor Microsoft Graph apelate de aplicația dvs. Permisiunile cu cele mai puțin privilegii, recomandate sunt furnizate în toate subiectele despre metoda de referință API Microsoft Graph. În plus, aceste permisiuni trebuie să fie acordate aplicației de către un utilizator sau un administrator. Acordarea permisiunilor are loc în mod normal printr-o pagină de consimțământ sau prin utilizarea blade-ului de înregistrare a aplicației Portal Azure. Din blade **Setări** pentru aplicație, faceți clic pe **Permisiuni necesare**, apoi faceți clic pe **Permisiuni**. Pentru mai multe informații, consultați:

- [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Înțelegerea permisiunilor și a consimțământului Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Eroare 403 Interzis: Aplicația dvs. a achiziționat un token pentru a se potrivi cu permisiunile alese?**

Asigurați-vă că tipurile de permisiuni solicitate sau acordate se potrivesc cu tipul de token de acces achiziționat de aplicație. Poate că solicitați și acordați permisiuni de aplicație, dar utilizați tokenuri de flux de cod interactiv delegate în locul tokenurilor de flux de acreditări client, sau solicitați și acordați permisiuni delegate, dar utilizați tokenuri de flux de acreditări client în locul tokenurilor de flux de cod delegate.

Pentru mai multe informații legate de achiziționarea de tokenuri, consultați:

- [Obțineți acces în numele utilizatorilor și permisiuni delegate](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - Fluxul de cod de autorizare OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obțineți acces fără un utilizator (serviciul daemon) și permisiuni de aplicație](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - Fluxul de acreditări client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Eroare 403 Interzis: Resetarea parolei**

În prezent, nu există permisiuni serviciu-la-serviciu daemon pentru aplicații care să permită resetarea parolelor utilizatorilor. Aceste API-uri sunt acceptate doar prin utilizarea fluxurilor de cod interactiv delegate cu un administrator conectat. Pentru mai multe informații, consultați [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Interzis: Utilizatorul are acces și are licență?**

Pentru fluxurile de cod delegate, Microsoft Graph evaluează dacă solicitarea a fost permisă pe baza permisiunilor acordate aplicației și a permisiunilor deținute de utilizatorul conectat. În general, această eroare indică faptul că utilizatorul nu are suficiente privilegii pentru a efectua solicitarea **sau** utilizatorul nu are licență pentru datele accesate. Numai utilizatorii cu permisiunile sau licențele necesare pot efectua solicitarea cu succes.

**403 Interzis: Ați selectat API-ul de resurse corect?**

Servicii API precum Microsoft Graph verifică dacă solicitarea *aud* (publicul) din tokenul de acces primit se potrivește cu valoarea pe care o așteaptă pentru sine și, dacă nu, apare o eroare 403 Interzis. O greșeală comună care rezultă din această eroare o constituie încercarea de a utiliza un token achiziționat pentru API-uri Azure AD Graph, API-uri Outlook sau API-uri SharePoint/OneDrive pentru a apela Microsoft Graph (sau invers). Asigurați-vă că resursa (sau domeniul) pentru care aplicația dvs. achiziționează un token se potrivește cu API-ul apelat de aplicație.

**400 Solicitare incorectă sau 403 Interzis: Utilizatorul respectă politicile de acces condiționat (CA) ale organizației sale?**

Pe baza politicilor de acces condiționat (CA) ale unei organizații, unui utilizator care accesează resursele Microsoft Graph prin aplicația dvs. i se pot solicita informații suplimentare care nu sunt prezente în tokenul de acces achiziționat inițial de aplicația dvs. În acest caz, aplicația dvs. primește o eroare **400 cu o eroare *interaction_required*** în timpul achiziției tokenului de acces, sau o eroare **403 cu o eroare *insufficient_claims*** la apelarea Microsoft Graph. În ambele cazuri, răspunsul de eroare conține informații suplimentare care pot fi prezentate la punctul final autorizat, pentru a solicita utilizatorului informații suplimentare (precum autentificare multi-factor sau înregistrarea dispozitivului).

Pentru mai multe informații despre accesul condiționat, consultați:

- [Gestionarea provocărilor de acces condiționat utilizând MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Îndrumări pentru dezvoltatori pentru accesul condiționat la Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Sfârșitul perioadei de asistență pentru biblioteca de autentificare Azure Active Directory (ADAL) și Azure AD Graph API (AAD Graph)_* _

- Începând cu 30 iunie 2020, nu vom mai adăuga caracteristici noi la biblioteca de autentificare Azure Active Directory (ADAL) și Azure AD Graph API (AAD Graph). Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.
- Începând cu 30 iunie 2022, vom înceta asistența pentru ADAL și AAD Graph, și nu vom mai furniza asistență tehnică sau actualizări de securitate.
    - Aplicațiile care utilizează ADAL în versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor primi asistență tehnică sau actualizări de securitate.
    - Este posibil ca aplicațiile care utilizează AAD Graph după această dată să nu mai primească răspunsuri de la punctul final AAD Graph.

_ *Migrarea ADAL**

Vă recomandăm să actualizați la [Biblioteca de autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), care are cele mai recente caracteristici și actualizări de securitate. Această recomandare vine în contextul migrării de către Microsoft a aplicațiilor sale în MSAL până la sfârșitul datei limită pentru asistență. Obiectivul migrării aplicațiilor Microsoft la MSAL este să ne asigurăm că aplicațiile beneficiază de îmbunătățirile permanente ale securității și caracteristicilor MSAL.

- [Citiți întrebările frecvente despre ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Aflați cum să efectuați migrarea aplicațiilor pe fiecare platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Dacă aveți nevoie de ajutor pentru a înțelege care dintre aplicațiile dvs. utilizează ADAL, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați oricare distribuitor de software independent (ISV) sau furnizor de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.

**Migrarea AAD Graph**

Pentru aplicațiile care utilizează AAD Graph, urmați instrucțiunile noastre pentru [migrarea aplicațiilor Azure AD Graph în Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Lista noastră de verificarea migrării oferă un punct de pornire](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portalul de înregistrare a aplicațiilor Azure afișează ce aplicații utilizează AAD Graph. Vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. și, dacă este cazul, să contactați orice furnizor de software independent sau furnizor de aplicații. Asistența Microsoft vă poate furniza, de asemenea, informații despre utilizarea AAD Graph în entitatea găzduită.

 










