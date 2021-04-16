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
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813736"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare de trimitere e-mail: Gazda client blocată utilizând Spamhaus

Adresa IP de la care a fost trimis mesajul se află pe o listă de blocări deținută [de Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Între motivele pentru blocarea de către Spamhaus sunt incluse conturi compromise, mașini compromise care partajează o adresă IP publică și politici ale unui furnizor de servicii internet (ISP). Remedierile posibile sunt:
  
- Pentru mesajele de intrare blocate, în care puteți controla serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocarea din site-ul web Spamhaus.

- Pentru mesajele de intrare către care adresa IP sursă aparține altcuiva, proprietarul adresei trebuie să elimine blocarea din site-ul web Spamhaus. Dacă adresa IP este pe Lista de blocare de politică (PBL - Policy Block List), proprietarul poate să atribuie o adresă IP statică diferită sau să elimine adresa din PBL.

- Pentru mesajele de ieșire blocate din domeniul dvs. conectat la Microsoft, puteți primi această eroare dacă mesajele sunt distribuite printr-un serviciu terț. Puteți utiliza un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.
