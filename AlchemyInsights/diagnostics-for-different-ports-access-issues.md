---
title: Diagnosticare pentru diferite probleme de acces la porturi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036811"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnosticare pentru diferite probleme de acces la porturi

Pentru a rezolva diferitele probleme de acces la porturi, efectuați pașii următori:

1. Opriți/dealocați mașina virtuală (VM) din portal, reporniți VM și testați din nou. 
2. Verificați setările de rețea din VM pentru a determina dacă aveți grupuri de securitate în rețea (NSGs) blocarea traficului. De asemenea, puteți să utilizați [Instrumentul de verificare a fluxului IP a rețelei Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) pentru a verifica dacă NSGs blocarea traficului, User-Defined rute (UDRs) redirecționarea traficului înapoi la local ("ruta implicită" 0.0.0.0/0) sau la un dispozitiv de rețea.
Dacă încă întâmpinați probleme după ce ați încercat pașii de mai sus, vă rugăm să furnizați numele VM și portul TCP în care încercați să trimiteți corespondența pentru un diagnostic suplimentar.

**Documente recomandate**

[Restricții și recomandări pentru trimiterea de mesaje de e-mail de ieșire prin portul 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)