---
title: Autentificare multi-factor neașteptată
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: d2b97175049bd9732b7444b029f7ea8610c3d5a2c02878ec5f20ded916baadd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53991151"
---
# <a name="unexpected-multi-factor-authentication"></a>Autentificare multi-factor neașteptată

Dacă entitatea dvs. găzduită a fost creată după 21 octombrie 2019 și vi se solicită în mod neașteptat pentru MFA, probabil că aveți [setările implicite de securitate](https://aka.ms/securitydefaults) activate în entitatea găzduită. 

Pentru a Gestiona setările implicite de securitate:

1. Conectați-vă la [centrul de administrare](https://go.microsoft.com/fwlink/p/?linkid=834822) utilizând acreditările de administrator Global.

2. Accesați [Proprietăți Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. În partea de jos a paginii, faceți clic pe **Gestionați Valorile Implicite de Securitate**.

4. Faceți clic pe **Da** pentru a activa setările implicite de securitate și **Nu** pentru a dezactiva setările implicite de securitate.
