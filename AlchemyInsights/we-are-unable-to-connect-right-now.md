---
title: Problema de activare-nu suntem în măsură să se conecteze chiar acum
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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628254"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Fixarea aplicațiilor Office "Suntem în imposibilitatea de a conecta chiar acum" mesaj

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați Paravanul de protecție, software-ul antivirus și setările proxy pentru a confirma că acestea nu blochează accesul la internet la aplicațiile Office. Consultați [Office 365 URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Du-te la **scrobeală** > a**alerga**, și apoi atunci tip **Services. msc**. Asigurați-vă că următoarele servicii se execută toate:
    - Instalare automată dispozitive conectate la rețea
    - Serviciu listă de rețea
    - Vizibilitate Locație rețea
    - Jurnal de evenimente Windows

Dacă unul dintre aceste servicii nu se execută, încercați să-l porniți. Dacă aveți o problemă la pornirea serviciului, executați următoarea comandă deschizând un prompt de comandă cu permisiuni elevate:

**SFC/scannow**

După terminarea acestei comenzi, reporniți computerul.

Pentru informații detaliate, consultați ["Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu "eroare atunci când activați Office din Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).