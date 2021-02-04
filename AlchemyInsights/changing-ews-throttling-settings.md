---
title: Modificarea setărilor de limitare EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075909"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="d02e2-102">Modificarea setărilor de limitare EWS</span><span class="sxs-lookup"><span data-stu-id="d02e2-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="d02e2-103">Rulați testul nostru automatizat, care vă va permite să modificați politica de limitare EWS pe durata migrării.</span><span class="sxs-lookup"><span data-stu-id="d02e2-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="d02e2-104">Rețineți că, și după rularea testului, importurile EWS vor fi în continuare limitate la 150 MB pe durata a 5 minute, pentru fiecare cutie poștală. Pentru a obține viteze mai mari de transfer al migrării, migrați mai mulți utilizatori simultan.</span><span class="sxs-lookup"><span data-stu-id="d02e2-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="d02e2-105">Rețineți că modificările politicii de limitare EWS nu au niciun efect asupra următoarelor tipuri de migrare (utilizând instrumente Microsoft): migrare hibridă, cu tranziție/pe etape (RPC/HTTP), IMAP, G Suite, Folder public sau Serviciu de import PST.</span><span class="sxs-lookup"><span data-stu-id="d02e2-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>