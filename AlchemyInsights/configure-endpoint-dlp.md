---
title: Configurați Microsoft Endpoint DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323930"
---
# <a name="configure-endpoint-dlp"></a>Configurați Microsoft Endpoint DLP

Microsoft Endpoint DLP vă permite să extindeți capacitatea de monitorizare și protecție DLP la informații confidențiale pe dispozitivele Windows 10. După înscrierea dispozitivelor în Gestionarea dispozitivelor, puteți crea politici DLP pentru a impune acțiuni de protecție pentru elemente. Exploratorul de activități poate fi utilizat pentru a monitoriza activitatea pentru elementele confidențiale. Pentru mai multe informații, consultați [Înscrierea dispozitivelor în Gestionarea dispozitivelor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Pentru a începe lucrul cu Microsoft Endpoint DLP:

- Asigurați-vă că aveți licențierea corespunzătoare pentru SKU/abonamente. Pentru mai multe informații, consultați [Licențierea pentru SKU/abonamente](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verificați permisiunile necesare pentru a activa gestionarea dispozitivelor, pentru accesa pagina de înscriere sau a activa/dezactiva monitorizarea dispozitivelor. Pentru mai multe informații, consultați [Permisiuni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Înscrieți dispozitive în Gestionarea dispozitivelor, urmând procedura pentru înscrierea dispozitivelor. Pentru mai multe informații, consultați [Înscrierea dispozitivelor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Creați politici DLP pentru a vă proteja elementele confidențiale. Pentru informații, consultați [Scenarii de politică Microsoft Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Pentru mai multe informații despre Microsoft Endpoint DLP, consultați [Aflați despre măsurile de prevenire a pierderii datelor Microsoft 365 Endpoint (previzualizare)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pași importanți de colectare a datelor, dacă este necesară asistența:**

1. Descărcați [previzualizarea analizorului client MDATP.](https://aka.ms/betamdatpanalyzer)
1. Rulați instrumentul ca administrator din fereastra cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Când vi se solicită să introduceți numărul de minute de colectare **a trasării:**, introduceți numărul de minute necesare pentru a rula scenariul.
1. Rulați scenariul.

Colectați rezultatul fișierului zip pentru a-l oferi agentului de asistență.
