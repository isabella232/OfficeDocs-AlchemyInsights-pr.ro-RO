---
title: Probleme la conectarea la aplicații
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901328"
---
# <a name="issues-signing-in-to-applications"></a>Probleme la conectarea la aplicații

Pentru a detecta cauzele sau diagnosticarea problemelor legate de conectarea la utilizator, efectuați pașii următori:

1. Lansați [diagnosticul de conectare](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Găsiți evenimentul de analizat introducând detaliile pe care le aveți despre utilizator, aplicație, ora conectării, ID-ul de solicitare sau ID-ul de corelare.
3. Revizuiți rezultatele de diagnosticare care afișează detaliile despre ce s-a întâmplat și ce acțiuni puteți efectua pentru a face modificări, dacă sunt necesare modificări.

Iată câteva probleme comune pe care le puteți întâmpina atunci când vă conectați la aplicații:

1. Dumneavoastră sau utilizatorul ați **finalizat o conectare AZURE AD, dar vedeți o solicitare neașteptată** -consultați articolul solicitarea de [consimțământ neașteptată atunci când vă conectați la o aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) și la o [Eroare neașteptată atunci când efectuați consimțământul pentru o aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Dumneavoastră sau un utilizator v **-ați conectat direct la o aplicație, dar nu vă puteți conecta la acesta de la un deeplink din portalul particularizat sau din panoul de acces**: consultați [Depanarea problemelor de conectare la o aplicație din Azure AD aplicațiile mele](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Dumneavoastră sau un utilizator ați **finalizat o conectare AZURE AD, dar aplicația afișează un mesaj de eroare și nu permite utilizatorului să termine fluxul de conectare**: problema este că aplicația nu a acceptat răspunsul pe care l-a emis Azure AD. Urmați [acești pași](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) pentru a depana.
4. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație non-Galerie configurată pentru sign-on unic pentru parole**: urmați instrucțiunile din [acești pași](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) pentru a depana.
5. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație AZURE AD Gallery configurată pentru sign-on unic pentru parole**: urmați [acești pași](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) pentru a depana.
6. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație Microsoft**: urmați [acești pași](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) pentru a depana.
7. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație non-Galerie configurată pentru sign-on unic federativ**: urmați [acești pași](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) pentru a depana.
8. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație AZURE AD Gallery configurată pentru sign-on unic federativ**: urmați [acești pași](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) pentru a depana.
9. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație dezvoltată la comandă**: urmați [acești pași](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) pentru a depana.
10. Dumneavoastră sau un utilizator **nu vă puteți conecta la o aplicație locală utilizând proxy-ul aplicației AZURE AD**: urmați [acești pași](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) pentru a depana.

