---
title: Problemă de activare - Nu ne putem conecta chiar acum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581887"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Fixarea microsoft 365 apps "Suntem în imposibilitatea de a conecta chiar acum" mesaj

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați setările paravanului de protecție, ale software-ului antivirus și proxy pentru a confirma că nu blochează accesul la Internet la aplicațiile Microsoft 365. Consultați [Adrese URL Microsoft și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Du-te la **Scrobeală**  >  **A alerga**, apoi apoi tip **services.msc**. Asigurați-vă că toate serviciile se execută:
    - Configurare automată dispozitive conectate la rețea
    - Serviciu listă de rețea
    - Vizibilitatea locației rețelei
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu funcționează, încercați să-l porniți. Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni privilegiate:

**sfc /scannow sfc / scannow sfc / scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" eroare atunci când activați Office de la Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).