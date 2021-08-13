---
title: Depanarea consimțământului utilizatorului
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007910"
---
# <a name="troubleshoot-user-consent"></a>Depanarea consimțământului utilizatorului

1. Puteți configura modul în care utilizatorii finali consimt ca utilizatorii finali să poată utiliza aplicațiile prin portalul Azure sau PowerShell. Consultați [Setările de consimțământ al](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) utilizatorului pentru mai multe informații.
1. De asemenea, un administrator poate [utiliza API-Graph Microsoft pentru](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) a acorda consimțământul delegatului în numele unui singur utilizator. Pentru mai multe informații, [consultați Obțineți acces în numele unui utilizator.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Erori de consimțământ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)al utilizatorului: acest articol prezintă erorile care pot apărea în timpul procesului de consimțământ pentru o aplicație. Dacă depanați solicitări de consimțământ neașteptate care nu conțin mesaje de eroare, consultați [Scenarii de autentificare pentru Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).