---
title: A apărut o eroare la validarea erorii tokenului de acces în timpul în care s-a făcut accesul la Desktop Analytics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946627"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Eroarea "A apărut o eroare la validarea tokenului de acces" în timpul însamblarii Analizei desktop

Această eroare se observă în mod normal atunci când tokenul de autentificare expiră. De obicei, reîmprospătarea paginii reîmprospătează tokenul. Cu toate acestea, această problemă poate persista dacă există politici de acces condiționat aplicate la contul utilizat la analiza desktop de la nivel de utilizator. Puteți revizui jurnalele de conectare Azure AD în portalul Azure pentru a vedea dacă există erori de conectare pentru contul utilizat pentru desktop Analytics de înscriere.

Pentru mai multe informații despre accesul condiționat, vizitați [Planificarea implementării accesului condiționat.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)