---
title: Eroare la validarea accesării simbolului de acces pe desktop Analytics la îmbarcare
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741250"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"A existat o eroare de validare a simbolului de acces" eroare în timpul desktop Analytics punerea

Această eroare se observă în mod normal atunci când expiră simbolul de autentificare. De obicei, reîmprospătarea paginii reîmprospătează simbolul. Cu toate acestea, această problemă poate persista dacă există orice politici de acces condiționat aplicate la contul utilizat la bord desktop Analytics. Aveți posibilitatea să examinați jurnalele de autentificare Azure AD în portalul Azure pentru a vedea dacă există erori de sign in pentru contul utilizat pentru desktop Analytics onboarding.

Pentru mai multe informații despre acces condiționat, vizitați [planul de implementare condițională de acces](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).