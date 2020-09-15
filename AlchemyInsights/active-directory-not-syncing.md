---
title: Active Directory nu se sincronizează
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697641"
---
# <a name="active-directory-not-syncing"></a>Active Directory nu se sincronizează

Dacă primiți erori de sincronizare, cum ar fi "fără sincronizare recentă" sau observați starea de sincronizare a directorului în portalul de administrare Office spune "Ultima sincronizare cu mai mult de 3 zile în urmă", este posibil ca AADConnect să aibă setări incorecte sau permisiuni insuficiente pentru a efectua o sincronizare.  

Reinstalarea AADConnect utilizând setările expres poate rezolva rapid problema:

1. [Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Urmați instrucțiunile pentru instalarea expres](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Pentru mai multe informații despre conturile de serviciu AADConnect, consultați [AZURE AD Connect: conturi și permisiuni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
