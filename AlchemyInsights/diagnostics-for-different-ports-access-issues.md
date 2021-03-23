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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="0fb3b-102">Diagnosticare pentru diferite probleme de acces la porturi</span><span class="sxs-lookup"><span data-stu-id="0fb3b-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="0fb3b-103">Pentru a rezolva diferitele probleme de acces la porturi, efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="0fb3b-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="0fb3b-104">Opriți/dealocați mașina virtuală (VM) din portal, reporniți VM și testați din nou.</span><span class="sxs-lookup"><span data-stu-id="0fb3b-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="0fb3b-105">Verificați setările de rețea din VM pentru a determina dacă aveți grupuri de securitate în rețea (NSGs) blocarea traficului.</span><span class="sxs-lookup"><span data-stu-id="0fb3b-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="0fb3b-106">De asemenea, puteți să utilizați [Instrumentul de verificare a fluxului IP a rețelei Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) pentru a verifica dacă NSGs blocarea traficului, User-Defined rute (UDRs) redirecționarea traficului înapoi la local ("ruta implicită" 0.0.0.0/0) sau la un dispozitiv de rețea.</span><span class="sxs-lookup"><span data-stu-id="0fb3b-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="0fb3b-107">Dacă încă întâmpinați probleme după ce ați încercat pașii de mai sus, vă rugăm să furnizați numele VM și portul TCP în care încercați să trimiteți corespondența pentru un diagnostic suplimentar.</span><span class="sxs-lookup"><span data-stu-id="0fb3b-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="0fb3b-108">**Documente recomandate**</span><span class="sxs-lookup"><span data-stu-id="0fb3b-108">**Recommended Documents**</span></span>

[<span data-ttu-id="0fb3b-109">Restricții și recomandări pentru trimiterea de mesaje de e-mail de ieșire prin portul 25</span><span class="sxs-lookup"><span data-stu-id="0fb3b-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)