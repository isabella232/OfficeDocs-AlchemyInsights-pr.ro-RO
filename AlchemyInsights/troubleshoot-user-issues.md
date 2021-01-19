---
title: Depanarea problemelor cu utilizatorul
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901335"
---
# <a name="announcements"></a>Anunțuri

Urmăriți Ghidul Google pentru testarea compatibilității pentru a testa dacă aplicațiile sunt afectate. Ghidul Google este disponibil în https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Asigurați-vă că utilizați vizualizarea web sau browserul de sistem la conectarea utilizatorilor cu conturi Google pentru consumatori. Pentru mai multe informații, consultați [probleme la conectarea la aplicații utilizând doar browserul Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Nu pot crea un utilizator nou în directorul Azure AD**

Pentru a depana problema de a nu putea crea un utilizator nou în Azure AD, efectuați pașii următori:

1. Asigurați-vă că sunteți autorizat să creați un nou utilizator standard. Doar rolul administratorului general sau al administratorului de utilizator din Azure Active Directory (AD) poate crea un nou utilizator standard. Dacă nu sunteți într-unul dintre aceste roluri, solicitați unui administrator să vă adauge la unul dintre aceste roluri sau să vă creeze noul cont de utilizator.
2. Asigurați-vă că numele de utilizator se află într-un domeniu care este verificat în reclama Azure. Dacă nu aveți niciun nume de domeniu particularizat verificat în reclama Azure, puteți utiliza domeniul inițial Azure AD, care se termină cu *. onmicrosoft.com.
3. Asigurați-vă că numele de utilizator se află într-un domeniu care nu este federativ la Azure AD din reclama locală. Utilizatorii nu pot fi adăugați în cloud cu numele de domenii care sunt federative din local.
4. Asigurați-vă că niciun alt utilizator sau persoană de contact nu are deja numele de utilizator pe care doriți să-l atribuiți noului utilizator. Numele de utilizator trebuie să fie unice în Azure AD.
5. Consultați [rolurile AZURE AD și administratorii](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pentru reclama Azure.
6. Consultați [numele de domenii](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) pentru reclama Azure.
7. Revizuiți [jurnalele de audit](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) pentru a vedea mai multe informații detaliate despre un utilizator recent creat sau șters, cum ar fi cine a efectuat acțiunea și când.
8. Pentru mai multe informații despre adăugarea de utilizatori noi, consultați [utilizarea portalului Azure pentru a crea un utilizator nou în reclama Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Pentru mai multe informații despre permisiunile pentru rolul de administrator din Azure AD, consultați [rolurile administrative AZURE AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Pentru detalii despre crearea unui utilizator utilizând Azure AD PowerShell, consultați [AZURE AD PowerShell pentru a crea un utilizator nou](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problemă cu înregistrarea cu autoservire**

Pentru a depana problemele legate de înregistrarea cu autoservire, efectuați pașii următori:

1. Pentru a utiliza înregistrarea cu autoservire cu aplicațiile, activați mai întâi înregistrarea cu autoservire pentru entitatea găzduită. 
2. Pentru a activa o aplicație pentru a accepta înregistrarea cu autoservire, adăugați-o la fluxul de utilizator. Data viitoare când accesați pagina de conectare pentru acea aplicație, veți vedea o opțiune **_fără cont? Creați unul!_* _. Aceasta pornește procesul de înregistrare cu autoservire.
3. Pentru informații despre cum să utilizați înregistrarea cu autoservire pentru a popula o organizație în Azure AD, consultați înscriere cu autoservire [pentru AZURE AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. După ce asociați fluxul de utilizator cu una sau mai multe aplicații, utilizatorii care vizitează acea aplicație se vor putea înregistra și pot obține un cont de invitat utilizând opțiunile configurate în fluxul de utilizatori. Pentru mai multe informații despre înregistrarea și obținerea unui cont de invitat, utilizatorii pot vedea înregistrarea cu autoservire [pentru utilizatorii invitați](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

*Problemă la invitarea unui utilizator extern**

Pentru a depana problemele legate de invitarea unui utilizator extern, efectuați următorul pas:

Asigurați-vă că trimiteți invitația unui utilizator la adresa de e-mail care se potrivește cu numele cu care se conectează utilizatorul. Dacă trimiteți invitația la adresa de e-mail a unui utilizator proxy, utilizatorul nu o poate valorifica. Pentru mai multe informații, consultați secțiunea [AZURE AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Nu pot atribui licențe unui utilizator**

Pentru a depana problemele legate de atribuirea de licențe unui utilizator, efectuați pașii următori:

1. Pentru a gestiona licențele de utilizator, asigurați-vă că utilizați un cont cu unul dintre rolurile de administrator necesare: administrator global, administrator de licență sau administrator de utilizator. Puteți să verificați rolul utilizatorului în fila **rol Director** de pe lama utilizatorului.
2. Dacă utilizați portalul Azure și atribuirea licenței nu reușește, faceți clic pe notificarea din colțul din dreapta sus. Aceasta deschide o lamă cu detalii despre ce nu a funcționat corect. În majoritatea cazurilor, este suficient să înțelegeți și să rezolvați problema.
3. Înainte ca o licență să fie atribuită unui utilizator, asigurați-vă că proprietatea **locației de utilizare** este setată pentru utilizator. Verificați dacă utilizatorul are acea proprietate setată prin vizualizarea filei de **profil** de pe lama de utilizator.
4. Asigurați-vă că există suficiente licențe disponibile pentru produsul pe care încercați să-l atribuiți. Puteți vedea numărul de licențe disponibile în portalul Azure, de la [Azure Active Directory-> licențe-> toate produsele](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Este posibil ca utilizatorul să aibă deja o altă licență ale cărei servicii intră în conflict cu cele din noua licență pe care încercați să o atribuiți. De exemplu, dacă utilizatorul are activat serviciul Exchange Online (plan 1), nu veți putea să atribuiți o licență cu Exchange Online (plan 2). Dezactivați unul dintre servicii pentru a permite noua atribuire a licenței. Dacă utilizați cmdleturi Azure portal sau PowerShell, pagina **Detalii problemă** listează anumite servicii care cauzează conflictul.
6. Dacă încercați să eliminați o licență și aceasta nu reușește, utilizatorul poate avea alte licențe cu servicii care depind de serviciile pe care încercați să le eliminați. Dacă utilizați cmdleturi Azure portal sau PowerShell, mesajul de eroare va lista serviciile specifice care au dependențe.
7. Dacă doriți să înțelegeți de ce a fost adăugată/eliminat o licență de la un utilizator (de exemplu, cine altcineva din organizație poate să fi efectuat modificări), Verificați jurnalele de auditare. Setați filtrul la **activitățile de licență** pentru a afișa toate modificările, inclusiv "Actorul" care le-a efectuat.
8. Dacă utilizați Exchange Online, unii utilizatori din entitatea găzduită pot fi configurați incorect cu aceeași valoare de adresă proxy. În astfel de cazuri, este posibil să vedeți mesaje de eroare generice atunci când o operațiune de licență nu reușește. [Acest articol](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) conține mai multe informații despre această problemă, inclusiv informații despre [cum să vă conectați la Exchange Online folosind PowerShell la distanță](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Pentru a identifica utilizatorii din entitatea găzduită, care conțin aceeași adresă proxy, executați acest cmdlet Exchange Online:

Fugi

Get-Recipient | Unde {$ _. EmailAddresses-Match <user principal name> } | fL name, RecipientType, EmailAddresses





