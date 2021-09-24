---
title: Nu puteți adăuga un cont după ce faceți upgrade la macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506754"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Nu puteți adăuga un cont după ce faceți upgrade la macOS 11.6 Big Sur

După ce faceți upgrade la macOS 11.6, contul dvs. OneDrive pentru locul de muncă sau de la școală sau contul dvs. personal OneDrive poate să nu apară în lista de conturi și este posibil să nu vă puteți conecta la un al doilea cont din aplicație.

O remediere a fost dezvoltată pentru această problemă. Mai întâi, determinați dacă rulați versiunea de OneDrive:

- Selectați meniul OneDrive cloud din bara de meniu > **Ajutor & Setări**  >  **Preferințe**  >  **Despre**. Dacă numărul de versiune nu include **(independent),** aveți versiunea de App Store a produsului.

Dacă utilizați versiunea independenta de OneDrive, reporniți computerul și OneDrive o actualizare automată la o compilare unde este rezolvată această problemă. Dacă doriți să instalați manual compilarea, descărcați acest fișier [.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), dezarhivarea fișierului și copiați aplicația OneDrive în folderul Aplicații (înlocuind aplicația OneDrive existentă).

Dacă utilizați versiunea App Store, luați în considerare instalarea versiunii OneDrive. Această versiune funcționează la fel ca versiunea din App Store, dar permite Microsoft să ofere actualizări mai rapid utilizatorilor și să le conecteze la o versiune care include remedierea pentru această problemă.

1. Descărcați versiunea OneDrive [de fișiere care include remedierea](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Dezarhivarea fișierului și copierea OneDrive fișier în folderul Aplicații (înlocuind aplicația OneDrive existentă).

Dacă trebuie să utilizați versiunea app Store, așteptați ca App Store să lanseze o versiune a aplicației care include remedierea. Din păcate, Microsoft nu poate comunica o dată estimată pentru lansarea unei versiuni fixe din App Store.


