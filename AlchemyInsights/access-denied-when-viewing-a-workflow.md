---
title: Acces refuzat la vizualizarea unui flux de lucru
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687342"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acces refuzat la vizualizarea unui flux de lucru

Fluxuri de lucru SharePoint 2013 care încearcă să trimită un e-mail la un grup SharePoint poate să nu reușească cu un mesaj de eroare "Access Denied" dacă apartenența la grupul SharePoint nu este setată la toată lumea.
  
 **Pentru a rezolva această problemă, efectuați acești pași:**
  
 1. Permiteți tuturor să vadă membrii grupului SharePoint.
  
 2. Eliminați grupul SharePoint din linia Către sau CC a e-mailului.
  
 3. Adăugați în mod explicit utilizatorii la linia Către sau CC dacă vizibilitatea apartenență nu poate fi modificată pentru grupul SharePoint.
  
Pentru a vizualiza mai multe detalii, vă rugăm să consultați [HTTP Neautorizat la /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  