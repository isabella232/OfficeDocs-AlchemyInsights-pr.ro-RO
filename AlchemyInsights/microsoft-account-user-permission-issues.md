---
title: Depanarea problemei - Utilizatorul nu a fost găsit în director
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098182"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Depanarea problemei - Utilizatorul nu a fost găsit în director

Dacă utilizatorii primesc mesajul de eroare "Utilizatorul nu poate fi găsit" în director, încercați din nou dacă Tipul de problemă este Utilizator care nu se află în director.

Următorii pași pot fi finalizați pentru a depana problema.

- Asigurați-vă că acel cont care a acceptat invitația prin e-mail este același cont care este utilizat pentru a vă conecta mai târziu. Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a se conecta la site. 

Pentru mai multe informații, [consultați Cum se gestionează aliasurile pentru contul Microsoft </a> pentru a gestiona Microsoft 365 conectare.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Navigați la fiecare site sau site în care utilizatorul primește eroarea. 

Adăugați "/_layouts/15/people.aspx/membershipgroupid=0" (în ghilimele duble) la sfârșitul adresei URL a site-ului. 

Exemplu: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selectați utilizatorul din listă.

- Faceți **clic pe Eliminare permisiuni utilizator** din panglică. 
-  Adăugați din nou Utilizatorul și retrimiteți invitația către utilizator.

