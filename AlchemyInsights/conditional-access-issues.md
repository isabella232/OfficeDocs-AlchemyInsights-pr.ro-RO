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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069976"
---
# <a name="conditional-access-issues"></a>Probleme de acces condiționat

**Rezolvarea problemelor cu Diagnostic de conectare**

Puteți afla rapid ce [s-a](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)întâmplat sau puteți diagnostica problemele legate de conectarea utilizatorilor utilizând Diagnostic de conectare:

1. Lansați Diagnostice de conectare.
1. Găsiți evenimentul de analizat, introducând detaliile pe care le aveți despre utilizator, aplicație, ora de conectare, ID-ul de solicitare sau ID-ul de corelare.
1. Revizuiți rezultatele de diagnosticare care afișează detalii despre ce s-a întâmplat și ce acțiuni puteți lua pentru a efectua modificări (dacă sunt necesare modificări).

**Pașii pentru depanarea unei autentificare** 

1. Navigați la pagina de conectare Azure AD.
1. Filtrați autentificări după utilizator, interval de timp, aplicație, stare, aplicație client și așa mai departe.
1. Selectați un eveniment de conectare și vizualizați fila Acces condiționat pentru a vedea ce politici au fost evaluate.
1. Faceți clic pe rândul unei politici pentru a vizualiza detaliile politicii și a înțelege de ce s-a aplicat.

**Tools to troubleshoot a Conditional Access policy**

- Modul doar raport vă permite să evaluați o politică fără a afecta utilizatorii.
- Instrumentul De ce ar fi dacă vă permite să simulați evenimente de conectare și să vedeți ce politici se aplică.
- Insights de lucru și de raportare afișează impactul în timp real al fiecărei politici.

**Politicile de protecție de referință**

Politicile de protecție de referință au fost perimate. Acestea nu mai sunt impuse și în curând vor fi eliminate din portalul Azure. Vă recomandăm să activați [valorile implicite de securitate](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Pentru mai multe informații despre Accesul condiționat, consultați:

[Cele mai bune practici pentru accesul condiționat în Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locații în Acces condiționat](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
