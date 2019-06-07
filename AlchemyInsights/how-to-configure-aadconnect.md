---
title: 646 cum la spre configure AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752573"
---
# <a name="configure-sync-features"></a>Configurați sincronizare caracteristici

Azur AD Connect include mai multe caracteristici care sunt activate în mod implicit, sau puteţi activa mai tarziu. Unele funcții necesită configurare suplimentare în anumite medii.

- [Filtrarea](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limitele obiectele sunt sincronizate cu Azur AD. Mod implicit, tuturor utilizatorilor, contacte, grupuri, şi Windows 10 calculator conturi sunt sincronizate. Pot include sau exclude obiecte bazate pe domenii, Pension sau alte atribute.

- [Sincronizarea de hash parola](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincronizează hash parola din Active Directory local azuriu AD. Acest lucru permite de gestionare a parolei într-o singură locaţie, dar utilizează aceeaşi parolă în ambele locală şi nor medii. Pentru Active Directory este sursă de autoritate, puteţi utiliza propriile politici de parola.

- [(SSPR) de resetare a parolei autoservire](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite utilizatorilor pentru a reseta parolele în nor în timp ce încă aplică politica de parola dumneavoastră local.

- [Dispozitivul writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite dispozitivelor înregistraţi în Azur Anunţul să fi scris înapoi în Active Directory local astfel încât ele pot fi folosite pentru acces condiționat.

- [Prevenirea accidental şterge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) este activată implicit pentru a preveni prea multe obiecte simultan ştergeri (peste 500 de obiecte pe sincronizare). Puteţi modifica această setare pentru a satisface nevoile dvs.

- [Actualizarea automată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) este activată implicit pentru instalatii expres şi ajută la asigurarea versiunea de AD Azure Connect este întotdeauna curent.
