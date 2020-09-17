---
title: Eroare la trimiterea e-mailului blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783815"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare la trimiterea mesajelor de e-mail: gazdă client blocată utilizând Spamhaus

Adresa IP care a trimis mesajul se află într-o listă de blocări deținută de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivele pentru care sunt blocate de Spamhaus includ conturi compromise, mașini compromise care partajează o adresă IP publică și politici de furnizor de servicii Internet (ISP). Remedieri posibile sunt:
  
- Pentru mesajele de intrare blocate în care controlați serverul de e-mail sursă, trebuie să determinați cauza și să eliminați blocul din site-ul web Spamhaus.

- Pentru mesajele de intrare blocate în care adresa IP sursă aparține altei persoane, proprietarul adresei trebuie să elimine blocul din site-ul web Spamhaus. Dacă adresa IP este pe lista de politici Block (PBL), proprietarul poate atribui o altă adresă IP statică sau elimina adresa din PBL.

- Pentru mesajele de ieșire blocate din domeniul conectat la Microsoft, puteți primi această eroare dacă mesajele sunt direcționate prin intermediul unui serviciu 3rd party. Puteți utiliza un instrument de căutare WHOIS pentru a găsi proprietarul adresei IP blocate.
