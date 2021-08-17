---
title: Active Directory nu se sincronizează
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314216"
---
# <a name="active-directory-not-syncing"></a>Active Directory nu se sincronizează

Dacă primiți erori de sincronizare, cum ar fi "nicio sincronizare recentă" sau observați starea de sincronizare a directorului în portalul de administrare Office spune "Ultima sincronizare cu mai mult de 3 zile în urmă", poate fi faptul că AADConnect are setări incorecte sau permisiuni insuficiente pentru a efectua o sincronizare.  

Reinstalarea AADConnect utilizând setări expres ar putea rezolva rapid problema:

1. [Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Urmați instrucțiunile pentru instalarea expres.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect trebuie să fie instalat pe Windows Server 2012 sau o versiune mai recentă. Acest server trebuie să fie asociat la domeniu și poate fi un controler de domeniu sau un server membru. Pentru o listă completă de cerințe de Conectare azure ad și cerințe preliminare, consultați Cerințe preliminare pentru [azure ad Conectare.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Pentru mai multe informații despre conturile de serviciu AADConnect, [consultați Azure AD Conectare: Conturi și permisiuni.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
