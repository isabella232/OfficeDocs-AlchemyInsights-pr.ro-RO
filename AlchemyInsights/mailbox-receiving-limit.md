---
title: Impunerea limitei de primire a cutiilor poștale
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316037"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Impunerea limitei de primire a cutiilor poștale

Microsoft a început recent să a impus pragul pentru fiecare cutie poștală de 3600 de mesaje pe oră. Pentru mai multe informații, [consultați Exchange Online limite.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 care primesc peste 3600 de mesaje într-o oră sunt amânate pentru următoarele 60 de minute. 

În plus, limita perechilor expeditor-destinatar (SRP) care blochează mesajele primite de o cutie poștală de Microsoft 365 de la un anumit expeditor se aplică. Dacă un singur expeditor trimite un anumit expeditor peste 33% din pragul total sau 1200 de mesaje pe oră în derulare unui anumit destinatar, începe limita de facturare și cutia poștală nu mai acceptă mesaje de la acel expeditor. Rețineți că:

- Această limită este pentru mesajele de e-mail primite de la alte entități găzduite, local sau expeditori de internet.
- Livrarea e-mailului în cutia poștală este blocată pentru următoarele 60 de minute. 
- Expeditorii care primesc aceste cutii poștale primesc un raport de ne delivery (5.2.121 sau 5.2.122), care spune că respectiva cutie poștală a depășit pragul maxim de livrare. Intra-tenant (e-mailul din aceeași entitate găzduită) continuă să fie livrat.
- Atunci când se aplică limita derp sRP, cutia poștală de primire continuă să accepte mesaje de la alți expeditori.

Administratorii pot monitoriza activitatea curentă din cutiile poștale, accesând un raport nou și detaliile din centrul de administrare Exchange denumit "Cutii poștale care depășesc limitele de primire". Detaliile apar doar dacă o entitate găzduită are cutii poștale problemă, în timp ce raportul apare întotdeauna în tabloul de bord, dar este gol, cu excepția cazului în care o entitate găzduită are cutii poștale problemă.

Pentru mai multe informații despre limitele de primire detaliată, consultați [Cutiile poștale care depășesc detaliile limitelor de primire în noul EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Pentru mai multe informații despre depășirea limitelor de primire, consultați [Cutiile poștale care depășesc limitele de primire în noul EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)