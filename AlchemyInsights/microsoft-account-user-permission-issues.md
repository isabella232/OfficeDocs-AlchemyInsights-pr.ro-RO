---
title: Depanarea problemei-utilizatorul nu a fost găsit în directorul
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754204"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Depanarea problemei-utilizatorul nu a fost găsit în directorul

Dacă utilizatorii primesc mesaj de eroare "utilizatorul nu poate fi găsit" în directorul. Încercați din nou în cazul în care tipul de problemă este utilizator nu în director.

Următorii pași se pot finaliza pentru a depana problema.

- Asigurați-vă că contul care a acceptat invitația de e-mail este același cont care este utilizat pentru a face sign in mai târziu. Asigurați-vă că utilizatorul utilizează același cont pentru a accepta invitația și a vă conecta la site. 

Pentru mai multe informații, consultați [se gestionează aliasuri pentru</a> contul Microsoft pentru a gestiona Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Răsfoiți la fiecare site (e) în care utilizatorul primește eroarea. 

Adăugați "/_layout/15/People.aspx/MembershipGroupId = 0" (în ghilimele duble) până la sfârșitul adresei URL a site-ului. 

Exemplu: https://_ _ \ "Contosoa _ Gt_. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.

- Selectați utilizatorul din listă.

- Faceți clic pe **Eliminare permisiuni utilizator** din panglică. 
-  Adăugați înapoi utilizatorul și Retrimi invitația la utilizator.

