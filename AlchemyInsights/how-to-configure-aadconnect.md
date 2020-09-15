---
title: 646 cum se configurează AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704501"
---
# <a name="configure-sync-features"></a>Configurarea caracteristicilor de sincronizare

Azure AD Connect include mai multe caracteristici activate în mod implicit sau pe care le puteți activa mai târziu. Unele caracteristici necesită o configurare suplimentară în anumite medii.

- Limite de [Filtrare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obiectele sunt sincronizate cu Azure AD. În mod implicit, toți utilizatorii, persoanele de contact, grupurile și conturile de computer Windows 10 sunt sincronizate. Puteți să includeți sau să excludeți obiecte pe baza domeniilor, a sau a altor atribute.

- [Sincronizarea codului hash pentru parole](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizează codul hash al parolei din Active Directory local la Azure AD. Acest lucru permite gestionarea parolelor într-o singură locație, dar utilizarea aceleiași parole în medii locale și în cloud. Deoarece Active Directory este sursa autoritară, puteți utiliza propriile politici pentru parole.

- [Resetarea parolei cu autoservire (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite utilizatorilor să-și reseteze propriile parole în cloud în timp ce aplică în continuare Politica de parolă locală.

- [Writeback dispozitivelor](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite ca dispozitivele înregistrate din Azure AD să fie scrise înapoi în Active Directory local, astfel încât să poată fi utilizate pentru acces condiționat.

- [Prevenirea ștergerii accidentale](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată în mod implicit pentru a împiedica prea multe ștergeri de obiecte simultane (mai mult de 500 de obiecte per sincronizare). Puteți modifica această setare pentru a răspunde nevoilor organizației dvs.

- [Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) -ul automat este activat în mod implicit pentru instalările expres și vă ajută să vă asigurați că versiunea de Azure AD Connect este întotdeauna curentă.
