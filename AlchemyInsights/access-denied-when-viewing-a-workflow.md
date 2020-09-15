---
title: Access Denied când Vizualizați un flux de lucru
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688814"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access Denied când Vizualizați un flux de lucru

Fluxurile de lucru SharePoint 2013 care încearcă să trimită un mesaj de e-mail la un grup SharePoint pot eșua cu un mesaj de eroare "Access Denied" Dacă apartenența la grupul SharePoint nu este setată pentru toată lumea.
  
 **Pentru a rezolva această problemă, urmați acești pași:**
  
 1. Permiteți tuturor să vadă membrii grupului SharePoint.
  
 2. Eliminați grupul SharePoint din linia către sau CC a e-mailului.
  
 3. Adăugați în mod explicit utilizatorii la linia către sau CC dacă vizibilitatea apartenenței nu poate fi modificată pentru grupul SharePoint.
  
Pentru a vedea mai multe detalii, consultați [http neautorizat pentru/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  