---
title: Remedierea aplicațiilor Microsoft 365 Ne pare rău, avem mesaj de probleme temporare de server
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
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582715"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Remedierea microsoft 365 apps "Ne pare rău, avem probleme temporare server" mesaj

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați setările paravanului de protecție, ale software-ului antivirus și proxy pentru a confirma că nu blochează accesul la Internet la aplicațiile Microsoft 365. Consultați [URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Du-te la **Scrobeală**  >  **A alerga**, apoi apoi tip **services.msc**. Asigurați-vă că toate serviciile se execută:
    - Configurare automată dispozitive conectate la rețea
    - Serviciu listă de rețea
    - Vizibilitatea locației rețelei
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu funcționează, încercați să-l porniți. Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni privilegiate:

**sfc /scannow sfc / scannow sfc / scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" eroare atunci când activați](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).