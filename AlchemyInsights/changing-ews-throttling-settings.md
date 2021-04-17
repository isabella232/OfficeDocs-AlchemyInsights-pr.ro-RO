---
title: Modificarea setărilor de limitare EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818048"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="dd874-102">Modificarea setărilor de limitare EWS</span><span class="sxs-lookup"><span data-stu-id="dd874-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="dd874-103">Rulați testul nostru automatizat, care vă va permite să modificați politica de limitare EWS pe durata migrării.</span><span class="sxs-lookup"><span data-stu-id="dd874-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="dd874-104">Rețineți că, și după rularea testului, importurile EWS vor fi în continuare limitate la 150 MB pe durata a 5 minute, pentru fiecare cutie poștală. Pentru a obține viteze mai mari de transfer al migrării, migrați mai mulți utilizatori simultan.</span><span class="sxs-lookup"><span data-stu-id="dd874-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="dd874-105">Rețineți că modificările politicii de limitare EWS nu au niciun efect asupra următoarelor tipuri de migrare (utilizând instrumente Microsoft): migrare hibridă, cu tranziție/pe etape (RPC/HTTP), IMAP, G Suite, Folder public sau Serviciu de import PST.</span><span class="sxs-lookup"><span data-stu-id="dd874-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>