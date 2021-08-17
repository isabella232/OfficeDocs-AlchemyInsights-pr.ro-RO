---
title: Aplicația Autentificare
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082954"
---
# <a name="authentication-app"></a>Aplicația Autentificare

Dacă sunteți administrator global, puteți afla rapid ce [s-a](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)întâmplat sau puteți diagnostica problemele legate de conectarea utilizatorilor utilizând Diagnostice de conectare.

1. Începeți diagnosticele făcând clic pe butonul["Lansare diagnostic".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Găsiți evenimentul de analizat, introducând detaliile pe care le aveți despre utilizator, aplicație, ora de conectare, ID-ul de solicitare sau ID-ul de corelare.
1. Examinați rezultatele diagnosticului care afișează detalii despre ce s-a întâmplat și ce acțiuni puteți lua pentru a face modificări, dacă sunt necesare modificări.

**Verificați scenariul care este aplicabil:**

1. Dacă un utilizator nu primi o notificare push în aplicația Microsoft Authenticator, verificați dacă nu sunt afișate sub utilizatorii blocați MFA, așa cum este descris în Blocarea și [deblocarea utilizatorilor.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Dacă utilizatorul nu este blocat pentru MFA, dar nu primește o notificare push, poate deschide aplicația Microsoft Authenticator, ceea ce va extrage solicitările de aprobare în așteptare.
1. Ca metodă alternativă de conectare, utilizatorul poate, de asemenea, să faceți clic pe Conectare în alt mod și să aleagă utilizarea unui cod de verificare din aplicația mobilă.
1. Aplicația Microsoft Authenticator este singura metodă disponibilă pentru mai mulți utilizatori. [Aflați mai multe despre valorile implicite](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)de [securitate , Authenticator Întrebări frecvente](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) despre aplicații pentru întrebări frecvente și despre cum să le rezolvați.
 
**Videoclipuri recomandate**

[Cum să configurați aplicația Authenticator pe un telefon nou (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
