---
title: Problemă de activare - Nu vă putem conecta momentan
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998173"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Remedierea Microsoft 365 mesajele "Nu vă putem conecta momentan"

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați firewallul, software-ul antivirus și setările proxy pentru a confirma că nu blochează accesul la internet la Microsoft 365 aplicații. Consultați [Adrese URL și intervale de adrese IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Accesați **Start**  >  **Run**, apoi tastați **services.msc**. Asigurați-vă că toate serviciile următoare rulează:
    - Configurarea automată a dispozitivelor conectate la rețea
    - Serviciul Listă de rețea
    - Informații despre locația de rețea
    - Windows Jurnalul de evenimente

Dacă unul dintre aceste servicii nu rulează, încercați să îl porniți. Dacă aveți o problemă la pornirea serviciului, rulați următoarea comandă deschizând o linie de comandă cu permisiuni cu drepturi înălțimii:

**sfc /scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, [consultați "Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" atunci când activați Office din Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).