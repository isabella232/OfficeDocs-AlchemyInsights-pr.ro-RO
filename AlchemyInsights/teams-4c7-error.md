---
title: Eroare Teams 4c7
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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786681"
---
# <a name="4c7-error-in-microsoft-teams"></a>Eroare 4c7 în Microsoft Teams

Această eroare apare deoarece Microsoft Teams necesită autentificarea Forms. Când implementați Active Directory Federation Services (AD FS), autentificarea Formulare nu este activată în mod implicit pentru intranet. Dacă autentificarea integrată Windows nu reușește, vi se solicită să vă conectați utilizând autentificarea Forms.

Pentru a rezolva această problemă, activați autentificarea Forms utilizând utilitarul de completare snap-in AD FS Microsoft Management Console (MMC) pe computerul care are copia locală de Active Directory. Pentru a proceda astfel, urmați acești pași: 

1. În panoul de navigare, navigați **la Politici de autentificare**.
2. Sub **Acțiuni,** în panoul de detalii, **selectați Editare autentificare primară globală.**
3. Pe fila **Intranet,** selectați **Autentificare formulare.**
4. Selectați **OK** (sau **Se aplică**).