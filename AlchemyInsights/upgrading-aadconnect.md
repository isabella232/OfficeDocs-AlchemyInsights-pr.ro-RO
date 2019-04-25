---
title: 932 actualizarea AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389743"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade azuriu AD conecta

În mod implicit, actualizarea automată este activată pentru Azure Connect AD, care ajută pentru a vă asigura că rulaţi cea mai recentă versiune. Pentru a verifica setările de actualizare automată, utilizaţi cmdletul **Get-ADSyncAutoUpgrade** din PowerShell de AD Azure. Cmdlet va returna una dintre următoarele valori: 

- **Enabled**: actualizarea automată este activată.

- **Cu handicap**: upgrade-ul automat este dezactivat.

- **Suspendat**: sistemul nu mai este eligibil pentru a primi upgrade-uri automate. Nu pot configura această valoare; Acesta este situat în sistemul de. 

Pentru informaţii suplimentare, consultaţi [actualizarea automată](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Pentru a descărca cea mai recentă versiune de Azure AD Connect, du-te la [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
