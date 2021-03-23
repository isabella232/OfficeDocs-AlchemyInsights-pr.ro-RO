---
title: Lucrul cu bibliotecile de autentificare
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036871"
---
# <a name="working-with-authentication-libraries"></a>Lucrul cu bibliotecile de autentificare

Pentru a rezolva problema bibliotecii de autentificare Microsoft (MSAL), efectuați următorii pași recomandate:

1. **Lucrul cu MSAL**: [biblioteci de autentificare a platformelor Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -acest articol afișează asistența pentru bibliotecile de autentificare Microsoft pentru mai multe tipuri de aplicații. Include linkuri către codul sursă al bibliotecii; de unde să obțineți pachetul pentru proiectul aplicației dvs.; și dacă biblioteca acceptă conectarea la utilizator (autentificarea), accesul la API-uri web protejate (autorizare) sau ambele.

2. **Depanarea autentificării**: MSAL acceptă mai multe fluxuri de autentificare pentru utilizare în scenarii de aplicație diferite. În funcție de modul în care este construită aplicația client, MSAL poate utiliza unul sau mai multe fluxuri de autentificare acceptate de platforma de identitate Microsoft. Aceste fluxuri pot genera mai multe tipuri de jetoane și coduri de autorizare și necesită simboluri diferite pentru a le face să funcționeze.

3. **Simboluri de acces**: [simboluri de acces ale platformei de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -Aflați cum poate valida API-ul și utiliza creanțele dintr-un simbol Access. Toate documentația din acest articol, cu excepția cazului în care se menționează, se aplică doar la tokenurile emise pentru API-uri pe care le-ați înregistrat. Nu se aplică tokenurilor emise pentru API-urile deținute de Microsoft și nici acele simboluri nu pot fi utilizate pentru a valida modul în care platforma de identitate Microsoft va emite tokenuri pentru un API pe care îl creați.

**Sfârșitul asistenței pentru Azure Active Directory Authentication Library (monica)**

- **Începând cu 30 iunie 2020,** nu vom mai adăuga caracteristici noi la Monica și Azure AD Graph. Vom continua să oferim asistență tehnică și actualizări de securitate, dar nu vom mai furniza actualizări de caracteristici.
- **Începând cu 30 iunie, 2022,** vom încheia asistența pentru monica și Azure AD Graph și nu va mai oferi asistență tehnică sau actualizări de securitate.
- Aplicațiile care utilizează monica pe versiunile de sistem de operare existente vor continua să funcționeze după această dată, dar nu vor *primi nicio asistență tehnică sau actualizări de securitate*.
- Aplicațiile care utilizează Azure AD Graph după această dată nu mai pot primi răspunsuri de la punctul final Azure AD Graph.

**Migrarea monica**

- Vă recomandăm să actualizați la MSAL, care are cele mai recente caracteristici și actualizări de securitate.
- Dacă utilizați aplicațiile Microsoft, știți că Microsoft se află în procesul de migrare a aplicațiilor sale la MSAL până la termenul limită de finalizare a asistenței, asigurându-vă că va beneficia de securitatea în curs de desfășurare și de îmbunătățiri ale caracteristicii MSAL.

1. [Citiți întrebările frecvente](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)despre Monica.
2. [Aflați cum să migrați aplicațiile pe o bază per platformă](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Dacă, după ce citiți Ghidul pentru platforma aplicației dvs., aveți întrebări suplimentare, puteți să postați pe [Microsoft Q&a](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) cu eticheta [Azure-AD-monica-dezaprobare] sau să deschideți o problemă în depozitul GitHub din bibliotecă. Consultați secțiunea [limbi și cadre](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) din articolul **Prezentare generală MSAL** pentru linkuri la repo pentru fiecare bibliotecă.
4. **Dacă aveți nevoie de ajutor pentru a înțelege ce aplicații utilizați** Monica, vă recomandăm să revizuiți toate codurile sursă ale aplicațiilor dvs. Dacă este cazul, contactați orice furnizor de software independent (ISV) sau furnizori de aplicații. De asemenea, asistența Microsoft vă poate oferi o listă a tuturor aplicațiilor ADAL care nu provin de la Microsoft din entitatea găzduită.







