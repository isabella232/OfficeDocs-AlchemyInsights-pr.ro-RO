---
title: Eroare trimitere e-mail blocat de SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29485035"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Eroare trimitere e-mail: clientul gazdă blocat folosind Spamhaus

IP-ul care a trimis mesajul este pe o listă de bloc, deţinut de [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Motivele fiind blocate de Spamhaus includ conturi compromise, compromisă masini schimb o adresă IP publică și politici de furnizorul de servicii Internet (ISP). Remedierile posibile sunt:
  
- Pentru mesajele de intrare blocat la Office 365 în cazul în care aveţi de a controla sursa de server de e-mail, aveţi nevoie pentru a determina cauza şi de a elimina bloc din site-ul Spamhaus.
    
- Blocat mesaje de intrare la Office 365 în cazul în care adresa de IP a sursei aparţine altcuiva, adresa proprietarului trebuie să scoateţi blocul Spamhaus pe site-ul. Dacă adresa IP este pe lista de bloc Politica (PBL), proprietarul poate atribui o altă adresă IP statică sau elimina adresa de PBL.
    
- Pentru mesajele de ieşire blocate din domeniul Office 365, puteţi primi această eroare în cazul în care mesajele sunt dirijate printr-un serviciu de 3rd party. Utilizaţi un instrument de căutare WHOIS pentru a găsi proprietarul de adrese IP blocate.
    

