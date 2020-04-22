---
title: Remedierea aplicațiilor Office Ne pare rău, avem mesaj de probleme temporare de server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764129"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Remedierea office apps "Ne pare rău, avem probleme temporare server" mesaj

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați setările paravanului de protecție, ale software-ului antivirus și ale proxy-ului pentru a confirma că nu blochează accesul la Internet la aplicațiile Office. Consultați [URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Du-te la **Scrobeală** > **A alerga**, apoi apoi tip **services.msc**. Asigurați-vă că toate serviciile se execută:
    - Configurare automată dispozitive conectate la rețea
    - Serviciu listă de rețea
    - Vizibilitatea locației rețelei
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu funcționează, încercați să-l porniți. Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni privilegiate:

**sfc /scannow sfc / scannow sfc / scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" eroare atunci când activați](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).