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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901632"
---
# <a name="troubleshoot-user-consent"></a>Depanarea consimțământului utilizatorului

1. Puteți configura modul în care utilizatorii finali sunt consimțământul aplicațiilor prin portalul Azure sau PowerShell. Consultați [setările de consimțământ pentru utilizatori](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) pentru mai multe informații.
1. De asemenea, un administrator poate utiliza [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) pentru a acorda consimțământul permisiunilor delegate în numele unui singur utilizator. Pentru mai multe informații, consultați [Obțineți acces în numele unui utilizator](https://docs.microsoft.com/graph/auth-v2-user).
1. [Erorile de consimțământ pentru utilizator](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): acest articol discută despre erorile care pot apărea în timpul procesului de consimțire la o aplicație. Dacă depanați solicitările de consimțământ neașteptate care nu conțin mesaje de eroare, consultați [scenarii de autentificare pentru AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).