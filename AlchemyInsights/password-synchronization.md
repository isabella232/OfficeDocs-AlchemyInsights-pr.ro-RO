---
title: Sincronizare parole
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483081"
---
# <a name="password-synchronization"></a>Sincronizare parole

**Sincronizarea codului hash pentru parole nu funcționează deloc**

Unele probleme uzuale pe care le întâmpină clienții atunci când sincronizarea hash a parolelor nu funcționează sunt:

- Contul Active Directory utilizat de Azure AD Connect pentru a comunica cu Active Directory local nu îi este permis să **reproducă modificări de Director** și să **reproducă modificările directorului toate** permisiunile, necesare pentru sincronizarea parolelor-trebuie să remediați acest lucru prin acordarea acestor permisiuni la contul Active Directory.
- Sincronizarea codului hash pentru parole este dezactivată după ce un administrator a modificat metoda de Sign-In utilizator de la **sincronizarea parolelor** la o altă opțiune, cum ar fi **Federation cu AD FS** din Azure AD Connect Wizard-puteți remedia acest lucru prin reactivarea caracteristicii de **sincronizare a parolei hash** în Expertul Azure AD Connect.
- Problemă de conectivitate cu Active Directory local. De exemplu, unele controlere de domeniu nu sunt accesibile prin Azure AD Connect sau [porturile necesare](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) sunt blocate de Paravanul de protecție-trebuie să remediați această problemă, asigurându-vă că conectivitatea dintre serverul Azure AD Connect și Active Directory local funcționează corect.
- Serverul Azure AD Connect se află în prezent în modul de așteptare, ceea ce va determina ca serverul să nu poată face codul hash pentru parole-pentru a depana problema, urmați pașii descriși în secțiunea [Depanarea sincronizării parolelor cu sincronizarea AZURE AD Connect-nu se sincronizează parole](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Sincronizarea hash a parolei nu funcționează pentru unii dintre utilizatorii mei**

1. Dacă ați observat că parola hash nu se sincronizează pentru un utilizator, utilizați activitatea de **Depanare** din Azure AD Connect pentru a investiga și a rezolva problema. Efectuați următoarele activități:

    un. [Rularea activității de depanare în expert](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Utilizați cmdletul depanare pentru a investiga problema de sincronizare a parolelor hash pentru o utilizare specifică](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Obiectul de utilizator Active Directory local este activat pentru **utilizator trebuie să modifice parola la următoarea** opțiune de conectare. Atunci când această opțiune este activată, utilizatorului i se atribuie o parolă temporară și vi se va solicita să modificați parola la următorul logon. Azure AD Connect nu sincronizează parolele temporare cu Azure AD.

Pentru a rezolva problema de mai sus, efectuați oricare dintre următoarele activități:

- Solicitați utilizatorului să se conecteze la o aplicație locală (de exemplu, desktop Windows) și să modifice parola. Noua parolă va fi sincronizată cu Azure AD.
- Depuneți un administrator să actualizeze parola utilizatorului fără a permite **utilizatorului opțiunea să modifice parola la următorul log on** și să partajeze noua parolă cu utilizatorul.

3. Obiectul de utilizator Active Directory local **nu este configurat corect** pentru sincronizarea obiectelor sau sincronizarea parolelor. Pentru a depana această problemă, urmați pașii descriși în [sincronizarea hash a parolei cu sincronizarea AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







