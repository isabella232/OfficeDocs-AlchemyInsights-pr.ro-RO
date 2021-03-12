---
title: Probleme cu o resursă sau cu un director de serviciu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714083"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Probleme cu o resursă sau cu un director de serviciu

1. Dacă tocmai ați început, [aplicațiile și obiectele principale de serviciu din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) descrie înregistrarea aplicațiilor, obiectele aplicației și principalele servicii din Azure Active Directory: care sunt acestea, modul în care sunt utilizate și modul în care acestea sunt asociate între ele. Un scenariu cu mai multe entități găzduite este prezentat, de asemenea, pentru a ilustra relația dintre obiectul aplicației al unei aplicații și obiectele principale de serviciu corespunzătoare.
2. Puteți afla mai multe despre relația dintre aplicații și directori de servicii, citind [aplicațiile și obiectele principale de serviciu din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. Instrucțiuni [: utilizarea portalului pentru a crea o aplicație AZURE AD și un director de serviciu care pot accesa resursele](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) vă arată cum să creați o aplicație Azure Active Directory (Azure AD) și principală de serviciu care pot fi utilizate cu controlul Access bazat pe roluri.
4. Cu API-ul [principal de serviciu](https://docs.microsoft.com/graph/api/resources/serviceprincipal), puteți să gestionați prin programare instanțele aplicațiilor și să controlați ce poate face o aplicație în cadrul entității găzduite.
5. [tipul de resursă servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) listează toate proprietățile și metodele pentru tipul de resursă servicePrincipal.
6. [Diferențele de tip de resurse între AZURE AD Graph și Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) evidențiază diferențele dintre Azure AD Graph și Microsoft Graph. Afișează resursele care au nume diferite sau nu sunt disponibile; de asemenea, evidențiază resursele disponibile în versiunea beta de Microsoft Graph, dar nu și în versiunea v 1.0.

**Probleme cu utilizatorii invitați**

- [Pornire rapidă: adăugarea utilizatorilor invitați la director în portalul Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vă arată cum să adăugați un utilizator nou invitat la directorul Azure AD prin intermediul portalului Azure, să trimiteți o invitație și să vedeți cum arată procesul de răscumpărare al utilizatorului invitat.
- [Tutorial: crearea fluxurilor de utilizator în Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) vă arată cum să creați unele fluxuri de utilizatori recomandate utilizând portalul Azure. În cazul în care căutați informații despre cum să configurați un flux de parole de proprietar de resurse (ROPC) în aplicație, consultați Configurarea fluxului de acreditări pentru parola proprietarului de resurse în Azure AD B2C.
