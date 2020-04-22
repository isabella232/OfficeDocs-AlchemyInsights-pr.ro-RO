---
title: Depanarea problemei - Utilizatorul nu a fost găsit în director
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702750"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Depanarea problemei - Utilizatorul nu a fost găsit în director

Dacă utilizatorii primesc mesajul de eroare "utilizatorul nu poate fi găsit" în director, încercați din nou în cazul în care tipul de problemă este utilizatorul nu în director.

Următorii pași pot fi finalizate pentru a depana problema.

- Asigurați-vă că contul care a acceptat invitația de e-mail este același cont care este utilizat pentru a vă conecta mai târziu. Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a vă conecta la site. 

Pentru mai multe informații, consultați [Cum se</a> gestionează aliasurile pentru contul Microsoft pentru a gestiona conectarea Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Răsfoiți la fiecare site-uri în care utilizatorul primește eroarea. 

Adăugați "/_layouts/15/people.aspx/membershipgroupid=0" (în cadrul ghilimelelor duble) la sfârșitul URL-ului site-ului. 

Exemplu: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selectați utilizatorul din listă.

- Faceți clic pe **Eliminare permisiuni utilizator** din panglică. 
-  Adăugați înapoi utilizatorul și retrimite invitația la utilizator.

