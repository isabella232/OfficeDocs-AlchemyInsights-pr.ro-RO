---
title: 646 Cum se configurează AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963655"
---
# <a name="configure-sync-features"></a>Configurarea caracteristicilor de sincronizare

Azure AD Conectare include mai multe caracteristici activate implicit sau pe care le puteți activa mai târziu. Unele caracteristici necesită o configurare suplimentară în anumite medii.

- [Limitele de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) filtrare Obiectele sunt sincronizate cu Azure AD. Implicit, toți utilizatorii, persoanele de contact, grupurile și conturile Windows 10 computer sunt sincronizate. Puteți să includeți sau să excludeți obiecte pe baza domeniilor, AE sau a altor atribute.

- [Sincronizarea hash-ului](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) parolelor sincronizează hash-ul parolei din Active Directory local cu Azure AD. Acest lucru permite gestionarea parolelor într-o singură locație, dar utilizarea aceleiași parole atât în mediile local, cât și în mediile în cloud. Deoarece Active Directory este sursa de autoritate, vă puteți utiliza propriile politici de parolă.

- [Resetarea parolei cu autoservire (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) le permite utilizatorilor să își reseteze propriile parole în cloud, aplicând în continuare politica de parole local.

- [Writebackul dispozitivelor](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite ca dispozitivele înregistrate în Azure AD să fie scrise în Active Directory local, astfel încât să poată fi utilizate pentru acces condiționat.

- [Prevenirea ștergerii accidentale](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată în mod implicit pentru a preveni ștergerile simultane ale obiectelor (peste 500 de obiecte per sincronizare). Puteți să modificați această setare pentru a răspunde nevoilor organizației dvs.

- [Upgrade-ul](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) automat este activat în mod implicit pentru instalările expres și vă ajută să vă asigurați că versiunea dvs. de Azure AD Conectare este întotdeauna curentă.
