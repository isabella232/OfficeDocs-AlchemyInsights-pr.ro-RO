---
title: Active Directory nu se sincronizează
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265268"
---
# <a name="active-directory-not-syncing"></a>Active Directory nu se sincronizează

Dacă primiți erori de sincronizare, ar fi nici o sincronizare recentă, sau observați starea de sincronizare director în portalul de administrare Office spune, Ultima sincronizat mai mult de 3 zile în urmă, este posibil ca AADConnect are setări incorecte sau insuficiente permisiuni pentru a efectua o sincronizare.  

Reinstalarea AADConnect utilizând setările expres poate rezolva problema rapid:

1. [Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Urmați instrucțiunile de instalare expres](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Pentru mai multe informații despre conturile de serviciu AADConnect, consultați [Azure AD Connect: Conturi și permisiuni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
