---
title: 646 se configurează AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722575"
---
# <a name="configure-sync-features"></a>Configurarea caracteristicilor de sincronizare

Azure AD conecta include mai multe caracteristici care sunt activate în mod implicit sau care se pot activa mai târziu. Unele caracteristici necesită configurare suplimentară în anumite medii.

- [Filtrarea](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limitelor obiectele sunt sincronizate cu Azure AD. În mod implicit, toți utilizatorii, persoanele de contact, grupurile și conturile de computer Windows 10 sunt sincronizate. Aveți posibilitatea să includeți sau să excludeți obiecte bazate pe domenii, o-uri sau alte atribute.

- [Sincronizarea hash parola](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizează hash parola din Active Directory local la Azure AD. Acest lucru permite gestionarea parolelor într-o singură locație, dar utilizarea aceleiași parole atât în mediul local, cât și în cel în cloud. Deoarece Active Directory este sursa cu autoritate, aveți posibilitatea să utilizați propriile politici de parolă.

- [Resetarea parolei cu autoservire (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite utilizatorilor să își reseteze propriile parole în cloud în timp ce aplică în continuare politica locală privind parolele.

- [Dispozitiv writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite dispozitive înregistrate în Azure AD pentru a fi scris înapoi la active directory local, astfel încât acestea să poată fi utilizate pentru acces condiționat.

- [Împiedicați ștergerea accidentală](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată în mod implicit pentru a preveni prea multe ștergeri simultane ale obiectelor (mai mult de 500 de obiecte per sincronizare). Aveți posibilitatea să modificați această setare pentru a satisface nevoile organizației.

- [Upgrade-ul automat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) este activat în mod implicit pentru instalările expres și vă ajută să vă asigurați că versiunea azure AD connect este întotdeauna curentă.
