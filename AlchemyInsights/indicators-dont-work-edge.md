---
title: Indicatorii nu funcționează utilizând browserul Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676464"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indicatorii nu funcționează utilizând browserul Edge

După ce ați creat un indicator, acesta nu este onorat de Edge (Smartscreen). Pentru mai multe informații, [consultați Crearea indicatorilor pentru URL-uri și URL-uri/domenii.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Pasul 1: Asigurați-vă de următoarele

- Verificați dacă indicatorul este corect (fără tastare în IP/URL, acțiune corectă, grupurile RBAC corecte).
- Așteptați minimum 2 ore după crearea indicatorului pentru a lua în considerare orice latență posibilă.
- Confirmați că sistemele sunt instalate în Microsoft Defender pentru punct final.
- Verificați dacă sistemele pot comunica cu cloud.
- Verificați dacă Smartscreen este activat și accesibil, dacă ajungeți la [site-ul de test](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Pasul 2: Depanați problema potențială

- Asigurați-vă că clientul îndeplinește cerințele. Pentru detalii, consultați [Crearea indicatorilor pentru URL-uri și URL-uri/domenii.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Asigurați-vă că rulați cea mai recentă versiune a browserului Edge. Pentru a afla cea mai recentă versiune, [consultați A afla ce versiune de Microsoft Edge aveți](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Reporniți browserul Edge.
- Navigați la site-ul pentru care ați configurat un indicator. Dacă site-ul nu apare așa cum vă așteptați, continuați cu Pasul 3. 

## <a name="step-3-collect-data"></a>Pasul 3: Colectarea datelor

- Colectați **date de diagnosticare MDEClientAnalyzer.** Pentru instrucțiuni, consultați [Probleme cu mașinile de bord la Microsoft Defender pentru punct final.](issues-with-onboarding-machines.md)
- Dacă sunteți confortabil să instalați și să colectați o urmărire Fiddler, consultați [Telerik Fiddler](http://www.telerik.com/fiddler).
- Dacă preferați instrucțiuni de la Asistența Microsoft, selectați pictograma Asistență de mai jos pentru a deschide un caz de asistență.
