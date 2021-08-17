---
title: 932 Upgrade-ul AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104824"
---
# <a name="upgrade-azure-ad-connect"></a>Faceți upgrade la Azure AD Conectare

În mod implicit, upgrade-ul automat este activat pentru azure ad Conectare, ceea ce vă ajută să vă asigurați că rulați cea mai recentă versiune. Pentru a verifica setările de upgrade automat, utilizați cmdletul **Get-ADSyncAutoUpgrade** din Azure AD PowerShell. Cmdletul va returna una dintre următoarele valori:

- **Activat:** Upgrade-ul automat este activat.

- **Dezactivat:** Upgrade-ul automat este dezactivat.

- **Suspendat:** Sistemul nu mai este eligibil pentru a primi upgrade-uri automate. Nu puteți configura această valoare; este setat de sistem.

Pentru mai multe informații, consultați [Upgrade-ul automat.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

Pentru a descărca cea mai recentă versiune de Azure AD Conectare, accesați [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
