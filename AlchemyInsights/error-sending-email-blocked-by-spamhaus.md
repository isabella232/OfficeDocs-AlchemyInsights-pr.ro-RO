---
title: Eroare la trimiterea e-mailului blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714270"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare la trimiterea e-mailului: Client gazdă blocat folosind Spamhaus

Adresa IP care a trimis mesajul este pe o listă de bloc deținute de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivele pentru care a fost blocat de Spamhaus includ conturi compromise, mașini compromise care partajează o adresă IP publică și politici de furnizor de servicii internet (ISP). Remedierile posibile sunt:
  
- Pentru mesajele de intrare blocate în cazul în care controlați serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocul de pe site-ul Web Spamhaus.

- Pentru mesajele de intrare blocate în cazul în care adresa IP sursă aparține altcuiva, proprietarul adresei trebuie să elimine blocul de pe site-ul Web Spamhaus. Dacă adresa IP se află în Lista de blocărărilor de politici (PBL), proprietarul poate atribui o altă adresă IP statică sau poate elimina adresa din PBL.

- Pentru mesajele de ieșire blocate din domeniul conectat la Microsoft, puteți primi această eroare dacă mesajele sunt distribuite printr-un serviciu terț. Utilizați un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.
