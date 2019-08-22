---
title: Acces interzis atunci când vizualizaţi un flux de lucru
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495835"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Acces interzis atunci când vizualizaţi un flux de lucru

SharePoint 2013 fluxurile de lucru care încerca să trimiteţi un email la un grup SharePoint poate eşua cu un mesaj de eroare "Access Denied" în cazul în care calitatea de membru al grupului de SharePoint nu este setată la toată lumea.
  
 **Pentru a rezolva această problemă, efectuaţi aceşti paşi:**
  
 1. Permite toată lumea să vadă membrii grup SharePoint.
  
 2. Elimina grup SharePoint de către sau CC linie de e-mail.
  
 3. Adăugaţi în mod explicit utilizatorilor către sau CC linie în cazul în care vizibilitatea aderarea nu poate fi schimbat pentru grup SharePoint.
  
Pentru a vizualiza mai multe detalii vă rugăm să consultaţi [HTTP neautorizat la /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  