---
title: Eroare de trimitere a e-mailului blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946778"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare de trimitere e-mail: Gazda client blocată utilizând Spamhaus

Adresa IP de la care a fost trimis mesajul se află pe o listă de blocări deținută [de Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Între motivele pentru blocarea de către Spamhaus sunt incluse conturi compromise, mașini compromise care partajează o adresă IP publică și politici ale unui furnizor de servicii internet (ISP). Remedierile posibile sunt:
  
- Pentru mesajele de intrare blocate, în care puteți controla serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocarea din site-ul web Spamhaus.

- Pentru mesajele de intrare către care adresa IP sursă aparține altcuiva, proprietarul adresei trebuie să elimine blocarea din site-ul web Spamhaus. Dacă adresa IP este pe Lista de blocare de politică (PBL - Policy Block List), proprietarul poate să atribuie o adresă IP statică diferită sau să elimine adresa din PBL.

- Pentru mesajele de ieșire blocate din domeniul dvs. conectat la Microsoft, puteți primi această eroare dacă mesajele sunt distribuite printr-un serviciu terț. Puteți utiliza un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.
