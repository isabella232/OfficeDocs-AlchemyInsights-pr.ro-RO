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
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402271"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare trimitere e-mail: clientul gazdă blocat folosind Spamhaus

IP-ul care a trimis mesajul este pe o listă de bloc, deţinut de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivele fiind blocate de Spamhaus includ conturi compromise, compromisă masini schimb o adresă IP publică și politici de furnizorul de servicii Internet (ISP). Remedierile posibile sunt:
  
- Pentru mesajele de intrare blocat la Office 365 în cazul în care aveţi de a controla sursa de server de e-mail, aveţi nevoie pentru a determina cauza şi de a elimina bloc din site-ul Spamhaus.
    
- Blocat mesaje de intrare la Office 365 în cazul în care adresa de IP a sursei aparţine altcuiva, adresa proprietarului trebuie să scoateţi blocul Spamhaus pe site-ul. Dacă adresa IP este pe lista de bloc Politica (PBL), proprietarul poate atribui o altă adresă IP statică sau elimina adresa de PBL.
    
- Pentru mesajele de ieşire blocate din domeniul Office 365, puteţi primi această eroare în cazul în care mesajele sunt dirijate printr-un serviciu de 3rd party. Utilizaţi un instrument de căutare WHOIS pentru a găsi proprietarul de adrese IP blocate.
    

