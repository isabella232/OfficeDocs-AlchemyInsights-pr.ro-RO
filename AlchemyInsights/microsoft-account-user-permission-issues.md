---
title: Depanarea problemei-utilizatorul nu a fost găsit în Director
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725419"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Depanarea problemei-utilizatorul nu a fost găsit în Director

Dacă utilizatorii primesc mesajul de eroare "utilizatorul nu poate fi găsit" în director, vă rugăm să încercați din nou în cazul în care tipul de problemă este utilizator care nu este în director.

Pașii următori pot fi terminați pentru a depana problema.

- Asigurați-vă că contul care a acceptat invitația de e-mail este același cont utilizat pentru a vă conecta mai târziu. Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a vă conecta la site. 

Pentru mai multe informații, consultați [cum să gestionați aliasuri pentru contul Microsoft </a> pentru a gestiona conectarea Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navigați la fiecare site-uri în care utilizatorul primește eroarea. 

Adăugați "/_layouts/15/People.aspx/MembershipGroupId = 0" (în ghilimele duble) până la sfârșitul URL-ului site-ului. 

Exemplu: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selectați utilizatorul din listă.

- Faceți clic pe **Eliminare permisiuni utilizator** din panglică. 
-  Adăugați înapoi utilizatorul și retrimiteți invitația la utilizator.

