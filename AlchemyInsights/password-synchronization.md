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
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960847"
---
# <a name="password-synchronization"></a>Sincronizare parole

**Sincronizarea parolelor cu hash nu funcționează deloc**

Câteva probleme comune pe care clienții le întâmpină atunci când nu funcționează sincronizarea parolelor cu hash sunt:

- Contului Active Directory utilizat de Azure AD Conectare pentru a comunica cu Active  Directory local  nu i se acordă modificări de director reproduse și modificări de director reproducere toate permisiunile necesare pentru sincronizarea parolei. Trebuie să remediați acest lucru acordând aceste permisiuni contului Active Directory.
- Sincronizarea parolelor hash este dezactivată după ce  un administrator a modificat metoda Sign-In de utilizator din sincronizarea parolelor la o altă opțiune, cum ar fi Federalizare cu **AD FS** din expertul Azure AD Conectare - Puteți remedia acest lucru activând din nou caracteristica de sincronizare a parolelor **hash** în expertul Azure AD Conectare.
- Problemă de conectivitate cu Active Directory local. De exemplu, unele controlere de domeniu nu sunt accesibile de [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) către Azure AD Conectare sau porturile necesare sunt blocate de Firewall, trebuie să remediați problema, asigurându-vă că conectivitatea dintre serverul Azure AD Conectare și Active Directory local funcționează corect.
- Serverul Azure AD Conectare se află în prezent în modul de testare, iar acest lucru va face ca serverul să nu poată avea erori hashe de parolă - Pentru a depana problema, urmați pașii descrisi în secțiunea Depanarea sincronizării parolelor cu sincronizarea [Azure AD Conectare -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Nu sunt sincronizate parole .

**Sincronizarea parolelor hash nu funcționează pentru unii dintre utilizatorii mei**

1. Dacă ați observat că nu se sincronizează  hash-ul parolei pentru un utilizator, utilizați activitatea de depanare din azure ad Conectare a investiga și a rezolva problema. Efectuați următoarele activități:

    a. [Rularea activității de depanare în expert](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Utilizați cmdletul de depanare pentru a investiga problema de sincronizare a hashului parolei pentru o anumită utilizare](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Obiectul Utilizator Active Directory local este activat pentru Utilizator trebuie să-și **schimbe parola la următoarea opțiune de** conectare. Atunci când această opțiune este activată, utilizatorului i se atribuie o parolă temporară și i se va solicita să modifice parola la următoarea conectare. Azure AD Conectare nu sincronizează parolele temporare cu Azure AD.

Pentru a rezolva problema de mai sus, efectuați oricare dintre următoarele activități:

- Cereți-i utilizatorului să se conecteze la aplicația locală (de exemplu, Windows desktop) și să modifice parola. Noua parolă va fi sincronizată cu Azure AD.
- Setați ca un administrator să actualizeze parola utilizatorului fără a activa opțiunea Utilizatorul trebuie să modifice parola la următoarea conectare și să partajeze parola nouă cu utilizatorul.

3. Obiectul Utilizator Active Directory local nu este configurat corect **pentru sincronizarea obiectelor** sau sincronizarea parolei. Pentru a depana această problemă, urmați pașii descrisi în Depanarea [sincronizării parolelor cu Azure AD Conectare sincronizare.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







