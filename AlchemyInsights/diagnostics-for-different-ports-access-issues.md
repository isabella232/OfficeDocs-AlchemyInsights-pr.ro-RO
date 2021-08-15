---
title: Diagnostics for different ports access issues
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030914"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostics for different ports access issues

Pentru a rezolva diferitele probleme de acces la port, efectuați pașii următori:

1. Opriți/alocate mașina virtuală (VM) din portal, reporniți VM și testați din nou. 
2. Verificați setările de rețea VM pentru a determina dacă aveți Grupuri de securitate de rețea (NSG) care blochează traficul. De asemenea, puteți utiliza instrumentul de verificare [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) al Verificator de rețea pentru a verifica dacă NSG blochează traficul, rute User-Defined (UDR) redirecționează traficul la local ('Default Route' 0.0.0.0/0) sau la un dispozitiv de rețea.
Dacă încă mai aveți probleme după ce încercați pașii de mai sus, furnizați numele de VM și portul TCP pe care încercați să trimiteți e-mailuri pentru alte adrese.

**Documente recomandate**

[Limitări și recomandări pentru trimiterea de e-mailuri de ieșire prin portul 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)