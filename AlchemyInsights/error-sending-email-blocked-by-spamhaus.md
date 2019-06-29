---
title: Eroare trimitere e-mail blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387861"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare trimitere e-mail: clientul gazdă blocat folosind Spamhaus

IP-ul care a trimis mesajul este pe o listă de bloc, deţinut de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivele fiind blocate de Spamhaus includ conturi compromise, compromisă masini schimb o adresă IP publică și politici de furnizorul de servicii Internet (ISP). Remedierile posibile sunt:
  
- Pentru mesajele de intrare blocat la Office 365 în cazul în care aveţi de a controla sursa de server de e-mail, aveţi nevoie pentru a determina cauza şi de a elimina bloc din site-ul Spamhaus.

- Blocat mesaje de intrare la Office 365 în cazul în care adresa de IP a sursei aparţine altcuiva, adresa proprietarului trebuie să scoateţi blocul Spamhaus pe site-ul. Dacă adresa IP este pe lista de bloc Politica (PBL), proprietarul poate atribui o altă adresă IP statică sau elimina adresa de PBL.

- Pentru mesajele de ieşire blocate din domeniul Office 365, puteţi primi această eroare în cazul în care mesajele sunt dirijate printr-un serviciu de 3rd party. Utilizaţi un instrument de căutare WHOIS pentru a găsi proprietarul de adrese IP blocate.
