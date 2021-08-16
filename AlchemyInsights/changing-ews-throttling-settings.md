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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968389"
---
# <a name="changing-ews-throttling-settings"></a>Modificarea setărilor de limitare EWS

Rulați testul nostru automatizat, care vă va permite să modificați politica de limitare EWS pe durata migrării. Rețineți că, și după rularea testului, importurile EWS vor fi în continuare limitate la 150 MB pe durata a 5 minute, pentru fiecare cutie poștală. Pentru a obține viteze mai mari de transfer al migrării, migrați mai mulți utilizatori simultan.

Rețineți că modificările politicii de limitare EWS nu au niciun efect asupra următoarelor tipuri de migrare (utilizând instrumente Microsoft): migrare hibridă, cu tranziție/pe etape (RPC/HTTP), IMAP, G Suite, Folder public sau Serviciu de import PST.