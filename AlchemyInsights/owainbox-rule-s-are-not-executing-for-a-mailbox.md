---
title: 1332 OWA - Inbox rule(s) sunt nu executa pentru o cutie poştală
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9e782faa59bb9a16c271f7c46c79635961e88aed
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30784353"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Regulă Inbox nu funcţionează conform aşteptărilor

Verificaţi următoarele setări:
  
- Un mesaj poate fi redirecţionat, altui tip de conþinut, sau a răspuns la automat bazat pe reguli Inbox numai o singură dată. O regulă de redirecţionare (o regulă Inbox sau mail fluxul de regulă, de asemenea, cunoscut ca o regulă de transport) puteţi adăuga maximum zece expediere destinatari la un mesaj. Pentru informaţii suplimentare, consultaţi [jurnal, Transport, şi Inbox limitele de regula](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Regulile pentru Inbox nu funcţionează pe cutia poştală de jurnalizare alternativ. Pentru mai multe informaţii despre cutia poştală de jurnalizare alternativă, a se vedea [poştală de jurnalizare alternativ](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Pentru a rezolva aceste probleme, a se vedea [KB 2829319](https://support.microsoft.com/kb/2829319).
  
În cazul în care problemele anterioare nu se aplică, executaţi raportul regulă Inbox de diagnosticare înainte să escaladeze emiterii către Microsoft Support:
  
1. Deschide cutia poştală în Outlook pe web, şi faceţi clic pe **Setări** \> **Opţiuni** \> **Organize e-mail** \> **regulile pentru Inbox**.
    
2. În partea de jos a paginii, faceţi clic pe **dacă regulile tale nu sunt de lucru faceţi clic aici pentru a genera un raport de diagnostic**.
    

