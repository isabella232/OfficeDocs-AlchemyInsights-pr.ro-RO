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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657941"
---
# <a name="configure-endpoint-dlp"></a>Configurați Microsoft Endpoint DLP

Microsoft Endpoint DLP vă permite să extindeți capacitatea de monitorizare și protecție DLP la informații confidențiale pe dispozitivele Windows 10. După înscrierea dispozitivelor în Gestionarea dispozitivelor, puteți crea politici DLP pentru a impune acțiuni de protecție pentru elemente. Exploratorul de activități poate fi utilizat pentru a monitoriza activitatea pentru elementele confidențiale. Pentru mai multe informații, consultați [Înscrierea dispozitivelor în Gestionarea dispozitivelor](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Pentru a începe lucrul cu Microsoft Endpoint DLP:

- Asigurați-vă că aveți licențierea corespunzătoare pentru SKU/abonamente. Pentru mai multe informații, consultați [Licențierea pentru SKU/abonamente](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verificați permisiunile necesare pentru a activa gestionarea dispozitivelor, pentru accesa pagina de înscriere sau a activa/dezactiva monitorizarea dispozitivelor. Pentru mai multe informații, consultați [Permisiuni](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Înscrieți dispozitive în Gestionarea dispozitivelor, urmând procedura pentru înscrierea dispozitivelor. Pentru mai multe informații, consultați [Înscrierea dispozitivelor](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Creați politici DLP pentru a vă proteja elementele confidențiale. Pentru informații, consultați [Scenarii de politică Microsoft Endpoint DLP](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Pentru mai multe informații despre Microsoft Endpoint DLP, consultați [Aflați despre măsurile de prevenire a pierderii datelor Microsoft 365 Endpoint (previzualizare)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pași importanți de colectare a datelor, dacă este necesară asistența:**

1. Descărcați [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Rulați instrumentul ca administrator din fereastra cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Când vi se solicită cu Introduceți numărul de minute de colectare a **trasării:**, introduceți numărul de minute necesare pentru a rula scenariul.
1. Rulați scenariul.

Colectați rezultatul fișierului zip pentru a-l oferi agentului de asistență.
