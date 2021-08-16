---
title: Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049320"
---
# <a name="4c7-error-in-microsoft-teams"></a>Eroare 4c7 în Microsoft Teams

Această eroare apare deoarece Microsoft Teams necesită autentificare Forms. Când implementați Active Directory Federation Services (AD FS), autentificarea Formulare nu este activată în mod implicit pentru intranet. Dacă Windows autentificarea integrată nu reușește, vi se solicită să vă conectați utilizând autentificarea forms.

Pentru a rezolva această problemă, activați autentificarea Forms utilizând utilitarul de completare snap-in AD FS Microsoft Management Console (MMC) pe computerul care are copia locală de Active Directory. Pentru a proceda astfel, urmați acești pași: 

1. În panoul de navigare, navigați **la Politici de autentificare**.
2. Sub **Acțiuni,** în panoul de detalii, **selectați Editare autentificare primară globală.**
3. Pe fila **Intranet,** selectați **Autentificare formulare.**
4. Selectați **OK** (sau **Se aplică**).