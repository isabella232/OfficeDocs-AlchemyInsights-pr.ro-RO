---
title: Aplicația mea nu se afișează în Guvernare aplicații
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454993"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Aplicația mea nu se afișează în Guvernare aplicații

Dacă aplicația dvs. nu se afișează în Guvernanță aplicații, verificați următoarele:

1. Accesați [Azure AD și găsiți](https://aad.portal.azure.com/) ID-ul aplicației dvs. căutând numele aplicației în bara de sus din pagina Prezentare generală.

1. Accesați Graph Explorer și căutați ID-ul aplicației în informațiile principale ale serviciului utilizând această interogare și înlocuind cu ID-ul relevant al <appId> aplicației: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Dacă nu se returnează niciun rezultat, căutați ID-ul aplicației în aplicație utilizând această interogare și înlocuind cu ID-ul relevant al <appId> aplicației: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Dacă aveți probleme cu interogarea, consultați [Obțineți asistență](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Pentru mai multe informații sau detalii despre aplicațiile dvs. în Guvernanța aplicațiilor, consultați [Aflați despre vizibilitate și detalii.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Pentru mai multe informații despre vizualizarea aplicațiilor, consultați [Vizualizarea aplicațiilor.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
