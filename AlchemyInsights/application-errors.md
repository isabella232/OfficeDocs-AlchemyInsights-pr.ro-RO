---
title: Erori de aplicație
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984661"
---
# <a name="application-errors"></a>Erori de aplicație

Căutați informații despre codurile de **Eroare AADSTS** care sunt returnate din serviciul token de securitate Azure Active Directory (Azure AD)? Citiți [codurile de eroare pentru autentificarea și autorizarea AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pentru a găsi descrieri de erori AADSTS, remedieri și câteva soluții sugerate.

Erorile de autorizare pot fi rezultatul mai multor probleme diferite, majoritatea generând o eroare 401 sau 403. De exemplu, următoarele pot duce la erori de autorizare:

- [Fluxuri de achiziție token Access](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorecte 
- [Domenii de permisiune](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) configurate slab 
- Lipsă de [consimțământ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Pentru a rezolva erorile comune de autorizare, încercați pașii furnizați mai jos, care se potrivesc cel mai bine cu eroarea pe care o primiți. Se pot aplica mai multe.

**eroare neautorizată 401: simbolul este valid?**

Asigurați-vă că aplicația prezintă un token de acces valid la Microsoft Graph ca parte a solicitării. Această eroare înseamnă adesea că simbolul de acces poate să lipsească din antetul de solicitare de autentificare HTTP sau că simbolul nu este valid sau a expirat. Vă recomandăm insistent să utilizați biblioteca de [autentificare Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) pentru achiziționarea de simboluri Access. În plus, această eroare poate apărea dacă încercați să utilizați un simbol de acces delegat acordat unui cont Microsoft personal pentru a accesa un API care acceptă doar conturile de la locul de muncă sau de la școală (conturi organizaționale).

**eroare interzisă 403: ați ales setul corect de permisiuni?**

Verificați dacă ați solicitat setul corect de permisiuni pe baza API-urilor Microsoft Graph pe care le apelează aplicația dvs. Permisiunile recomandate cel mai puțin privilegiat sunt furnizate în toate subiectele metodei de referință Microsoft Graph API. În plus, aceste permisiuni trebuie să fie acordate aplicației de către un utilizator sau de către un administrator. Acordarea permisiunilor se întâmplă în mod normal printr-o pagină de consimțământ sau prin acordarea de permisiuni utilizând lama de înregistrare a aplicației Azure portal. Din lama de **Setări** pentru aplicație, faceți clic pe **permisiuni necesare**, apoi faceți clic pe **acordare permisiuni**.

- [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Înțelegerea permisiunilor și consimțământului Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**eroare interzisă 403: aplicația a obținut un token pentru a se potrivi cu permisiunile alese?**

Asigurați-vă că tipul de permisiuni solicitat sau acordat se potrivește cu tipul de token de acces pe care îl dobândește aplicația dvs. Este posibil să solicitați și să acordați permisiuni de aplicație, dar să utilizați tokenuri de flux de cod interactiv delegate în locul tokenurilor flux de acreditare client sau să solicitați și să acordați permisiuni delegate, dar să utilizați tokenuri de flux de acreditare client în locul tokenurilor flux de cod delegate.

- [Obțineți acces în numele utilizatorilor și al permisiunilor delegate](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 codul de autorizare flux](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obțineți acces fără un utilizator (Serviciu Daemon) și permisiuni de aplicație](https://docs.microsoft.com/graph/auth_v2_service) 
- [Flux de acreditări client Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**eroarea interzisă 403: Reinițializarea parolei**

În prezent, nu există permisiuni de aplicație daemon service-to-service care permit reinițializarea parolelor utilizatorilor. Aceste API-uri sunt acceptate doar utilizând fluxurile de coduri interactive delegate cu un administrator conectat.

- [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 interzis: utilizatorul are acces și este licențiat?**

Pentru fluxurile de coduri delegate, Microsoft Graph evaluează dacă solicitarea este permisă în funcție de permisiunile acordate aplicației și de permisiunile pe care le are utilizatorul conectat. În general, această eroare indică faptul că utilizatorul nu este suficient de privilegiat pentru a efectua solicitarea sau că utilizatorul nu are licență pentru datele care se accesează. Numai utilizatorii cu permisiuni sau licențe necesare pot face solicitarea cu succes.

**403 interzis: ați selectat API-ul de resurse corect?**

Servicii API precum Microsoft Graph Verificați dacă afirmația aud (audiența) din simbolul Access primit se potrivește cu valoarea pe care o așteaptă de la sine și, dacă nu, aceasta are ca rezultat o eroare interzisă 403. O greșeală comună care rezultă din această eroare încearcă să utilizeze un token dobândit pentru API-uri Azure AD Graph, API-uri Outlook sau SharePoint/OneDrive pentru a apela Microsoft Graph (sau invers). Asigurați-vă că resursa (sau domeniul de aplicare) aplicația achiziționează un token pentru potrivește cu API-ul pe care îl solicită aplicația.

**400 Solicitare eronată sau 403 interzisă: utilizatorul respectă politicile de acces condiționat (CA) ale Organizației?**

Pe baza politicilor CA ale unei organizații, un utilizator care accesează resurse Microsoft Graph prin intermediul aplicației poate fi contestat pentru informații suplimentare care nu sunt prezente în tokenul Access pe care aplicația l-a achiziționat inițial. În acest caz, aplicația primește un 400 cu o eroare de *interaction_required* în timpul achiziționării tokenului de acces sau al unui 403 cu eroarea *insufficient_claims* atunci când se solicită Microsoft Graph. În ambele cazuri, răspunsul de eroare conține informații suplimentare care pot fi prezentate la punctul final autorizat pentru a contesta utilizatorul pentru informații suplimentare (cum ar fi autentificarea multi-factor sau înscrierea dispozitivelor).

- [Gestionarea provocărilor accesului condiționat utilizând MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Ghid pentru dezvoltatori pentru acces condițional Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
