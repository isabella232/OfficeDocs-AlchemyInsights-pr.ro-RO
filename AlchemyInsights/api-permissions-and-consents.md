---
title: Permisiunile API și Consimțământul
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932109"
---
# <a name="api-permissions-and-consent"></a>Permisiunile API și consimțământul

Aplicațiile care se integrează cu Serviciu de identitate Microsoft urmează un model de autorizare care le oferă utilizatorilor și administratorilor control asupra modului în care pot fi accesate datele. Implementarea modelului de autorizare a fost actualizată pe Serviciu de identitate Microsoft final. Aceasta schimbă modul în care o aplicație trebuie să interacționeze cu Serviciu de identitate Microsoft. [Permisiunile și consimțământul din punctul Serviciu de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) final acoperă conceptele de bază ale acestui model de autorizare, inclusiv domeniile, permisiunile și consimțământul.

Cadrul [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) facilitează dezvoltarea aplicațiilor client web cu mai multe entități găzduite și native. Aceste aplicații permit conectarea de către conturi de utilizator de la o entitate găzduită Azure AD, care sunt diferite de cea în care este înregistrată aplicația. De asemenea, poate fi necesar ca acestea să acceseze API-uri web, cum ar fi API Microsoft Graph (pentru a accesa Azure AD, Intune și serviciile în Microsoft 365) și alte API-uri servicii Microsoft, pe lângă API-urile web proprii.

