---
title: Permisiuni și consimțământ pentru API
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
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974991"
---
# <a name="api-permissions-and-consent"></a>Permisiuni și consimțământ pentru API

Aplicațiile care se integrează cu platforma de identitate Microsoft urmăresc un model de autorizare care le oferă utilizatorilor și administratorilor controlul asupra modului în care pot fi accesate datele. Implementarea modelului de autorizare a fost actualizată pe punctul final al platformei de identitate Microsoft. Acesta modifică modul în care o aplicație trebuie să interacționeze cu platforma de identitate Microsoft. [Permisiunile și consimțământul în punctul final al platformei de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) acoperă conceptele de bază ale acestui model de autorizare, inclusiv domeniile, permisiunile și consimțământul.

Framework-ul de [consimțământ Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) vă ajută să dezvoltați mai ușor aplicații client web și nativi cu mai mulți entități găzduite. Aceste aplicații permit conectarea de către conturile de utilizator de la o entitate găzduită Azure AD care diferă de cea în care este înregistrată aplicația. De asemenea, poate fi necesar să acceseze API-uri web, cum ar fi Microsoft Graph API (pentru a accesa Azure AD, Intune și Services în Microsoft 365) și alte API-uri de servicii Microsoft, în plus față de propriile API-uri web.

