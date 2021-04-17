---
title: Remedierea aplicațiilor Microsoft 365 Ne pare rău, avem mesaje de probleme temporare despre server
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835283"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Remedierea aplicațiilor Microsoft 365 Cu mesajul "Ne pare rău, avem probleme temporare pe server"

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați setările pentru firewall, software antivirus și proxy pentru a confirma că nu blochează accesul la internet la aplicațiile Microsoft 365. Consultați [URL-uri și intervale de adrese IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Accesați **Start**  >  **Run**, apoi tastați **services.msc**. Asigurați-vă că toate serviciile următoare rulează:
    - Configurarea automată a dispozitivelor conectate la rețea
    - Serviciul Listă de rețea
    - Informații despre locația de rețea
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu rulează, încercați să îl porniți. Dacă aveți o problemă la pornirea serviciului, rulați următoarea comandă deschizând o linie de comandă cu permisiuni cu drepturi înălțimii:

**sfc /scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, [consultați "Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" atunci când activați.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)