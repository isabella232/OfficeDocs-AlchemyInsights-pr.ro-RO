---
title: Acces refuzat atunci când vizualizați un Flux de lucru
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955213"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acces refuzat atunci când vizualizați un Flux de lucru

SharePoint 2013 Workflows care încearcă să trimită un mesaj de e-mail la un grup SharePoint pot să nu reușească cu un mesaj de eroare "Acces refuzat" dacă apartenența la grupul SharePoint nu este setată la Oricine.
  
 **Pentru a rezolva această problemă, urmați acești pași:**
  
 1. Permiteți tuturor să vadă membrii grupului SharePoint grup.
  
 2. Eliminați grupul SharePoint din linia Către sau CC a mesajului de e-mail.
  
 3. Adăugați în mod explicit utilizatorii în linia Către sau CC, dacă vizibilitatea apartenenței nu poate fi modificată SharePoint grup.
  
Pentru a vedea mai multe detalii, consultați [Http Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  