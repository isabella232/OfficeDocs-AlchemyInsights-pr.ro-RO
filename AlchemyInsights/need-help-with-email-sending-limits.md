---
title: Aveți nevoie de ajutor pentru trimiterea de e-mailuri limite?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357871"
---
# <a name="need-help-with-email-sending-limits"></a>Aveți nevoie de ajutor pentru trimiterea de e-mailuri limite?

Mai jos este **de-design trimiterea limitelor** aplicate în serviciu. Mai multe informații cu privire la aceste limite sunt documentate [aici](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- Pentru a descuraja livrarea de mesaje în bloc nesolicitate, aplicăm limitele de rată ale **destinatarului**per utilizator tuturor mesajelor de ieșire și interne . În toate SKU-urile, această limită este **de 10.000 de destinatari pe zi.**  Clienții care trebuie să trimită e-mailuri comerciale în bloc legitime (de exemplu, buletine informative pentru clienți) ar trebui să utilizeze furnizori terți specializați în aceste servicii.
    - **Notă:** Odată ce limita de rată a destinatarului este atinsă, mesajele nu pot fi trimise din cutia poștală până când numărul de destinatari cărora le-au fost trimise mesaje în ultimele 24 de ore scade sub limită. Utilizatorul nu va putea trimite mesaje până în acel moment.
- Limita ratei de mesaj de **30 de mesaje pe minut** se aplică în toate SKU-uri. Acest lucru determină câte mesaje poate trimite un utilizator din contul exchange online într-o perioadă specificată.
- **Numărul maxim de destinatari permis în câmpurile Către, Cc și Cci** pentru un singur mesaj de poștă electronică, în toate SKU-urile, este de **1000 de destinatari**. Pentru a particulariza această limită, mergeți [aici](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
