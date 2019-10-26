---
title: Acces refuzat la vizualizarea unui flux de lucru
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747760"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acces refuzat la vizualizarea unui flux de lucru

SharePoint 2013 fluxuri de lucru care încearcă să trimiteți un e-mail la un grup SharePoint poate eșua cu un mesaj de eroare "Access Denied" Dacă apartenența la grupul SharePoint nu este setată la toată lumea.
  
 **Pentru a rezolva această problemă, urmați acești pași:**
  
 1. Permiteți tuturor să vadă membrii grupului SharePoint.
  
 2. Eliminați grupul SharePoint din linia către sau CC a e-mailului.
  
 3. Adăugați în mod explicit utilizatorii la linia către sau CC dacă vizibilitatea apartenenței nu se poate modifica pentru grupul SharePoint.
  
Pentru a vedea mai multe detalii, vă rugăm să consultați [http neautorizat la/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  