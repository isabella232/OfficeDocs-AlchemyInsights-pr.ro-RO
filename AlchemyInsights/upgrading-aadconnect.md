---
title: 932 Actualizarea AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766505"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD Conectați

În mod implicit, upgrade-ul automat este activat pentru Azure AD Connect, ceea ce vă ajută să vă asigurați că executați cea mai recentă versiune. Pentru a verifica setările de upgrade automat, utilizați cmdletul **Get-ADSyncAutoUpgrade** în Azure AD PowerShell. Cmdletul va returna una dintre următoarele valori:

- **Activat:** Este activată upgrade-ul automat.

- **Dezactivat:** Upgrade-ul automat este dezactivat.

- **Suspendat:** Sistemul nu mai este eligibil pentru a primi upgrade-uri automate. Imposibil de configurat această valoare; Este setat de sistem.

Pentru mai multe informații, consultați [Upgrade automat](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pentru a descărca cea mai recentă versiune [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)de Azure AD Connect, accesați .
