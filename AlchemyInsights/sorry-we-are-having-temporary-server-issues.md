---
title: Remedierea aplicațiilor Microsoft 365 ne pare rău, avem mesaje temporare de probleme cu serverul
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758257"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Remedierea aplicațiilor Microsoft 365 "Ne pare rău, avem probleme cu serverul temporare"

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați firewallul, software-ul antivirus și setările proxy pentru a confirma că nu blochează accesul la internet la aplicațiile Microsoft 365. Vedeți [adresele URL și intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Accesați **Start**  >  **Run**, apoi tastați **Services. msc**. Asigurați-vă că toate următoarele servicii sunt în execuție:
    - Configurarea automată a dispozitivelor conectate la rețea
    - Serviciu listă de rețele
    - Conștientizarea locației rețelei
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu rulează, încercați să-l porniți. Dacă aveți o problemă la pornirea serviciului, derulează următoarea comandă deschizând o linie de comandă cu permisiuni ridicate:

**SFC/scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Vă rugăm să încercați din nou mai târziu "eroare la activare](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).