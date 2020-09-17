---
title: 932 upgrade-ul AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806051"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade-ul Azure AD Connect

În mod implicit, upgrade-ul automat este activat pentru Azure AD Connect, care vă ajută să vă asigurați că rulează cea mai recentă versiune. Pentru a verifica setările de upgrade automat, utilizați cmdletul **Get-ADSyncAutoUpgrade** din Azure AD PowerShell. Cmdletul va returna una dintre următoarele valori:

- **Activat**: upgrade-ul automat este activat.

- **Dezactivat**: upgrade-ul automat este dezactivat.

- **Suspendat**: sistemul nu mai este eligibil pentru a primi upgrade-uri automate. Nu puteți configura această valoare; este setat de sistem.

Pentru mai multe informații, consultați upgrade-ul [automat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pentru a descărca cea mai recentă versiune de Azure AD Connect, accesați [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
