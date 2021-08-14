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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931461"
---
# <a name="application-errors"></a>Erori de aplicație

Căutați informații despre codurile de eroare **AADSTS** returnate din serviciul de simboluri de securitate Azure Active Directory (Azure AD) (STS)? Citiți [Codurile de eroare](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pentru autentificarea și autorizarea Azure AD pentru a găsi descrierile erorilor AADSTS, remedierile și unele soluții sugerate.

Erorile de autorizare pot rezulta din mai multe probleme diferite, majoritatea generând o eroare 401 sau 403. De exemplu, următoarele pot duce la erori de autorizare:

- [Fluxuri de acces](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) incorecte 
- [Domenii de permisiune](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) incorect configurate 
- Lipsa [consimțământului](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Pentru a rezolva erorile de autorizare comune, încercați pașii furnizati mai jos care se potrivesc cel mai bine cu eroarea pe care o primiți. Se pot aplica mai multe.

**Eroare 401 Neautorizat: Tokenul dvs. este valid?**

Asigurați-vă că aplicația dvs. prezintă un token de acces valid pentru Microsoft Graph ca parte a solicitării. Această eroare înseamnă adesea că tokenul de acces poate lipsi din antetul solicitării HTTP de autentificare sau că tokenul nu este valid sau a expirat. Vă recomandăm ferm să utilizați Biblioteca de autentificare [Microsoft (MSAL) pentru achiziționarea tokenului](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) de acces. În plus, această eroare poate apărea dacă încercați să utilizați un token de acces delegat acordat unui cont Microsoft personal pentru a accesa un API care acceptă doar conturi de la locul de muncă sau de la școală (conturi de organizație).

**Eroare 403 Interzis: Ați ales setul corect de permisiuni?**

Verificați dacă ați solicitat setul corect de permisiuni pe baza api-ului Microsoft Graph API-urile aplicației. Permisiunile recomandate pentru cel mai puțin privilegiați sunt furnizate în toate subiectele despre metoda de Graph API Microsoft. În plus, aceste permisiuni trebuie să fie acordate aplicației de către un utilizator sau un administrator. Acordarea permisiunilor în mod normal se face printr-o pagină de consimțământ sau prin acordarea de permisiuni utilizând sistemul blade de înregistrare a aplicației Azure Portal. Din blade **Setări** pentru aplicație, faceți clic pe **Permisiuni necesare**, apoi faceți clic pe **Permisiuni**.

- [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Înțelegerea permisiunilor și a consimțământului Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Eroare 403 Interzis: Aplicația dvs. a achiziționat un token pentru a se potrivi cu permisiunile alese?**

Asigurați-vă că tipul de permisiuni solicitat sau acordat corespunde tipului de simbol de acces achiziționat de aplicație. Este posibil să solicitați și să acordți permisiuni pentru aplicație, dar utilizând simboluri de flux de cod interactive delegate în locul simbolurilor de flux de acreditări ale clientului sau solicitarea și acordarea permisiunilor delegate, dar utilizarea simbolurilor de flux de acreditări client în locul simbolurilor de flux de cod delegat.

- [Obțineți acces în numele utilizatorilor și permisiuni delegate](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - Fluxul de cod de autorizare OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Obțineți acces fără un utilizator (serviciul daemon) și permisiuni de aplicație](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - Fluxul de acreditări client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Eroare 403 Interzis: Resetarea parolei**

În prezent, nu există permisiuni serviciu-la-serviciu daemon pentru aplicații care să permită resetarea parolelor utilizatorilor. Aceste API-uri sunt acceptate doar prin utilizarea fluxurilor de cod interactiv delegate cu un administrator conectat.

- [Permisiuni Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Interzis: Utilizatorul are acces și are licență?**

Pentru fluxurile de cod delegate, Microsoft Graph evaluează dacă solicitarea este permisă pe baza permisiunilor acordate aplicației și a permisiunilor pe care le are utilizatorul conectat. În general, această eroare indică faptul că utilizatorul nu are suficiente privilegii pentru a efectua solicitarea sau utilizatorul nu are licență pentru datele accesate. Numai utilizatorii cu permisiunile sau licențele necesare pot efectua solicitarea cu succes.

**403 Interzis: Ați selectat API-ul de resurse corect?**

Servicii API precum Microsoft Graph verificați dacă solicitarea aud (audiență) din simbolul de acces primit se potrivește cu valoarea pe care o așteaptă pentru sine și, dacă nu, duce la o eroare 403 Forbidden. O greșeală comună care rezultă din această eroare o constituie încercarea de a utiliza un token achiziționat pentru API-uri Azure AD Graph, API-uri Outlook sau API-uri SharePoint/OneDrive pentru a apela Microsoft Graph (sau invers). Asigurați-vă că resursa (sau domeniul) pentru care aplicația dvs. achiziționează un token se potrivește cu API-ul apelat de aplicație.

**400 Solicitare incorectă sau 403 Interzis: Utilizatorul respectă politicile de acces condiționat (CA) ale organizației sale?**

Pe baza politicilor organizației, un utilizator care accesează resursele Microsoft Graph prin aplicația dvs. poate fi provocat pentru informații suplimentare care nu sunt prezente în simbolul de acces achiziționat inițial de aplicația dvs. În acest caz, aplicația dvs. primește o eroare 400 cu o eroare *interaction_required* în timpul achiziției tokenului de acces, sau o eroare 403 cu o eroare *insufficient_claims* la apelarea Microsoft Graph. În ambele cazuri, răspunsul la eroare conține informații suplimentare care pot fi prezentate punctului final autorizat să verificarea utilizatorului pentru informații suplimentare (cum ar fi Multi-Factor Authentication sau înscrierea dispozitivului).

- [Gestionarea provocărilor accesului condiționat utilizând MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Îndrumări pentru dezvoltatori pentru accesul condiționat la Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
