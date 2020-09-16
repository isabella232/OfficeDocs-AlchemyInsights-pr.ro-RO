---
title: Problemă de activare-nu ne putem conecta acum
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725995"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Remedierea aplicațiilor Microsoft 365 "nu ne putem conecta acum"

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați firewallul, software-ul antivirus și setările proxy pentru a confirma că nu blochează accesul la internet la aplicațiile Microsoft 365. Vedeți [adresele URL și intervalele de adrese IP Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Accesați **Start**  >  **Run**, apoi tastați **Services. msc**. Asigurați-vă că toate următoarele servicii sunt în execuție:
    - Configurarea automată a dispozitivelor conectate la rețea
    - Serviciu listă de rețele
    - Conștientizarea locației rețelei
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu rulează, încercați să-l porniți. Dacă aveți o problemă la pornirea serviciului, derulează următoarea comandă deschizând o linie de comandă cu permisiuni ridicate:

**SFC/scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Vă rugăm să încercați din nou mai târziu "eroare atunci când activați Office de la Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).