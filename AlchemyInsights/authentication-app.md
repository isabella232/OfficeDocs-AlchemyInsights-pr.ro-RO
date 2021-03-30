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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405678"
---
# <a name="authentication-app"></a>Aplicația Autentificare

Dacă sunteți administrator global, puteți afla rapid ce [s-a](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)întâmplat sau puteți diagnostica problemele legate de conectarea utilizatorilor utilizând Diagnostice de conectare.

1. Începeți diagnosticele făcând clic pe butonul["Lansare diagnostic".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Găsiți evenimentul de analizat, introducând detaliile pe care le aveți despre utilizator, aplicație, ora de conectare, ID-ul de solicitare sau ID-ul de corelare.
1. Examinați rezultatele diagnosticului care afișează detalii despre ce s-a întâmplat și ce acțiuni puteți lua pentru a face modificări, dacă sunt necesare modificări.

**Verificați scenariul care este aplicabil:**

1. Dacă un utilizator nu primi o notificare push în aplicația Microsoft Authenticator, verificați dacă nu este afișat sub utilizatorii blocați MFA, așa cum este descris în Blocarea și [deblocarea utilizatorilor.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Dacă utilizatorul nu este blocat pentru MFA, dar nu primește o notificare push, poate deschide aplicația Microsoft Authenticator, care va extrage solicitările de aprobare în așteptare.
1. Ca metodă alternativă de conectare, utilizatorul poate, de asemenea, să faceți clic pe Conectare în alt mod și să aleagă utilizarea unui cod de verificare din aplicația mobilă.
1. Aplicația Microsoft Authenticator este singura metodă disponibilă pentru mulți utilizatori. [Aflați mai multe despre valorile implicite de](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)securitate , consultați Întrebări frecvente despre aplicația [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) pentru întrebări frecvente și despre cum să le rezolvați.
 
**Videoclipuri recomandate**

[Cum să configurați aplicația Authenticator pe un telefon nou (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
