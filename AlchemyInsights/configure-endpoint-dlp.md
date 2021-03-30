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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402447"
---
# <a name="configure-endpoint-dlp"></a>Configurați Microsoft Endpoint DLP

Microsoft Endpoint DLP vă permite să extindeți capacitatea de monitorizare și protecție DLP la informații confidențiale pe dispozitivele Windows 10. După înscrierea dispozitivelor în Gestionarea dispozitivelor, puteți crea politici DLP pentru a impune acțiuni de protecție pentru elemente. Exploratorul de activități poate fi utilizat pentru a monitoriza activitatea pentru elementele confidențiale. Pentru mai multe informații, consultați [Înscrierea dispozitivelor în Gestionarea dispozitivelor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Pentru a începe lucrul cu Microsoft Endpoint DLP:

- Asigurați-vă că aveți licențierea corespunzătoare pentru SKU/abonamente. Pentru mai multe informații, consultați [Licențierea pentru SKU/abonamente](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Verificați permisiunile necesare pentru a activa gestionarea dispozitivelor, pentru accesa pagina de înscriere sau a activa/dezactiva monitorizarea dispozitivelor. Pentru mai multe informații, consultați [Permisiuni](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Înscrieți dispozitive în Gestionarea dispozitivelor, urmând procedura pentru înscrierea dispozitivelor. Dacă lipsește opțiunea Înscrierea dispozitivelor (previzualizare) sub Conformitate M365  **Setări**, confirmați că aveți licența și permisiunile corespunzătoare la care s-a făcut referire mai sus. Pentru mai multe informații, consultați [Înscrierea dispozitivelor](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Creați politici DLP pentru a vă proteja elementele confidențiale. Pentru informații, consultați [Scenarii de politică Microsoft Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Pentru mai multe informații despre Microsoft Endpoint DLP, consultați [Aflați despre măsurile de prevenire a pierderii datelor Microsoft 365 Endpoint (previzualizare)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Pași importanți de colectare a datelor, dacă este necesară asistența:**

1. Descărcați MDATP Client Analyzer Preview de la [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Rulați instrumentul ca administrator din fereastra cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Când vi se solicită „Introduceți numărul de minute pentru a colecta trasarea: ”, introduceți numărul de minute necesare pentru a rula scenariul
5. Rulați scenariul

Colectați rezultatul fișierului zip de trimis agentului de asistență.
