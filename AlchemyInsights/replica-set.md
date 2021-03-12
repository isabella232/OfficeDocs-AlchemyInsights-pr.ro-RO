---
title: Set de reproduceri
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714255"
---
# <a name="replica-set"></a>Set de reproduceri

AADDS este, de asemenea, denumit domeniul gestionat. De fapt, sunt două controlere de domeniu care rulează și sunt întreținute de backend. Cele două DCs includ un DC principal și unul de replicare DC. Backupurile din AADDS (domeniul gestionat) sunt un proces automatizat gestionat de platforma Azure. În cazul unei probleme cu domeniul gestionat, asistența Azure vă poate ajuta în restaurarea din backup.

Creați fiecare set de reproduceri într-o rețea virtuală. Fiecare rețea virtuală trebuie să fie coordonată fiecărei rețele virtuale care găzduiește un set de reproduceri al domeniului gestionat. Această configurație creează o topologie de rețea Mesh care acceptă reproducerea directorului. O rețea virtuală poate accepta mai multe seturi de replicare, cu condiția ca fiecare set de reproduceri să se află într-o subrețea virtuală diferită.

Pentru mai multe detalii despre setul de reproduceri, consultați [seturi de reproduceri concepte](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
