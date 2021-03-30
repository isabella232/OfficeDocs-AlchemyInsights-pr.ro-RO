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
# <a name="authentication-app"></a><span data-ttu-id="c58bf-102">Aplicația Autentificare</span><span class="sxs-lookup"><span data-stu-id="c58bf-102">Authentication app</span></span>

<span data-ttu-id="c58bf-103">Dacă sunteți administrator global, puteți afla rapid ce [s-a](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)întâmplat sau puteți diagnostica problemele legate de conectarea utilizatorilor utilizând Diagnostice de conectare.</span><span class="sxs-lookup"><span data-stu-id="c58bf-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="c58bf-104">Începeți diagnosticele făcând clic pe butonul["Lansare diagnostic".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="c58bf-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="c58bf-105">Găsiți evenimentul de analizat, introducând detaliile pe care le aveți despre utilizator, aplicație, ora de conectare, ID-ul de solicitare sau ID-ul de corelare.</span><span class="sxs-lookup"><span data-stu-id="c58bf-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="c58bf-106">Examinați rezultatele diagnosticului care afișează detalii despre ce s-a întâmplat și ce acțiuni puteți lua pentru a face modificări, dacă sunt necesare modificări.</span><span class="sxs-lookup"><span data-stu-id="c58bf-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="c58bf-107">**Verificați scenariul care este aplicabil:**</span><span class="sxs-lookup"><span data-stu-id="c58bf-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="c58bf-108">Dacă un utilizator nu primi o notificare push în aplicația Microsoft Authenticator, verificați dacă nu este afișat sub utilizatorii blocați MFA, așa cum este descris în Blocarea și [deblocarea utilizatorilor.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="c58bf-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="c58bf-109">Dacă utilizatorul nu este blocat pentru MFA, dar nu primește o notificare push, poate deschide aplicația Microsoft Authenticator, care va extrage solicitările de aprobare în așteptare.</span><span class="sxs-lookup"><span data-stu-id="c58bf-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="c58bf-110">Ca metodă alternativă de conectare, utilizatorul poate, de asemenea, să faceți clic pe Conectare în alt mod și să aleagă utilizarea unui cod de verificare din aplicația mobilă.</span><span class="sxs-lookup"><span data-stu-id="c58bf-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="c58bf-111">Aplicația Microsoft Authenticator este singura metodă disponibilă pentru mulți utilizatori.</span><span class="sxs-lookup"><span data-stu-id="c58bf-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="c58bf-112">[Aflați mai multe despre valorile implicite de](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)securitate , consultați Întrebări frecvente despre aplicația [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) pentru întrebări frecvente și despre cum să le rezolvați.</span><span class="sxs-lookup"><span data-stu-id="c58bf-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="c58bf-113">**Videoclipuri recomandate**</span><span class="sxs-lookup"><span data-stu-id="c58bf-113">**Recommended Videos**</span></span>

<span data-ttu-id="c58bf-114">[Cum să configurați aplicația Authenticator pe un telefon nou (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c58bf-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
