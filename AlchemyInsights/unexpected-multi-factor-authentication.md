---
title: Autentificare multi-factor neașteptată
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946734"
---
# <a name="unexpected-multi-factor-authentication"></a>Autentificare multi-factor neașteptată

Dacă entitatea dvs. găzduită a fost creată după 21 octombrie 2019 și vi se solicită în mod neașteptat pentru MFA, probabil că aveți [setările implicite de securitate](http://aka.ms/securitydefaults) activate în entitatea găzduită. 

Pentru a Gestiona setările implicite de securitate:

1. Conectați-vă la [centrul de administrare](https://go.microsoft.com/fwlink/p/?linkid=834822) utilizând acreditările de administrator Global.

2. Accesați [Proprietăți Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. În partea de jos a paginii, faceți clic pe **Gestionați Valorile Implicite de Securitate**.

4. Faceți clic pe **Da** pentru a activa setările implicite de securitate și **Nu** pentru a dezactiva setările implicite de securitate.
