---
title: Probleme de acces condiționat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014890"
---
# <a name="conditional-access-issues"></a>Probleme de acces condiționat

**Rezolvarea problemelor cu diagnosticul de conectare**

Puteți afla rapid ce s-a întâmplat sau cum să diagnosticați problemele legate de conectarea la utilizator, utilizând [diagnosticul de conectare](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Lansați diagnosticul de conectare.
1. Găsiți evenimentul de analizat introducând detaliile pe care le aveți despre utilizator, aplicație, ora conectării, ID-ul de solicitare sau ID-ul de corelare.
1. Revizuiți rezultatele de diagnosticare care afișează detaliile despre ce s-a întâmplat și ce acțiuni puteți efectua pentru a face modificări (dacă sunt necesare modificări).

**Pașii pentru depanarea unui sign in** 

1. Navigați la pagina de conectare la Azure AD.
1. Filtrați sign-in-uri după utilizator, interval de timp, aplicație, stare, aplicație client etc.
1. Selectați un eveniment de conectare și vizualizați fila acces condiționat pentru a vedea ce politici au fost evaluate.
1. Faceți clic pe rândul unei politici pentru a vizualiza detaliile politicii și a înțelege de ce s-a aplicat.

**Instrumente pentru a depana o politică de acces condiționat**

- Modul doar în raport vă permite să evaluați o politică fără a afecta utilizatorii.
- Instrumentul ce-If vă permite să simulați evenimentele de conectare și să vedeți ce politici se aplică.
- Detalii și registru de lucru raportare afișează impactul în timp real al fiecărei politici.

**Politici de protecție de referință**

Politicile de protecție de referință au fost dezaprobate. Acestea nu mai sunt impuse și vor fi eliminate în curând din portalul Azure. Vă recomandăm să activați [valorile implicite de securitate](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Pentru mai multe informații despre accesul condiționat, consultați:

[Cele mai bune practici pentru accesul condiționat din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Condiții în Access condițional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controale în Access condițional](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locații în Access condițional](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
