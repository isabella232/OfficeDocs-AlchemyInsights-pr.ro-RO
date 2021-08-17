---
title: Set de reproducere
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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110692"
---
# <a name="replica-set"></a>Set de reproducere

AADDS se mai numește și domeniu gestionat. De fapt, sunt două controlere de domeniu care sunt rulate și întreținute de backend. Cele două DCs includ un dc principal și o reproducere DC. Copiile backup din AADDS (domeniul gestionat) sunt un proces automatizat gestionat de platforma Azure. În cazul unei probleme cu domeniul gestionat, asistența Azure vă poate asista la restaurarea de pe backup.

Creați fiecare set de reproducere într-o rețea virtuală. Fiecare rețea virtuală trebuie să fie grupată la fiecare altă rețea virtuală care găzduiește setul de reproducere a unui domeniu gestionat. Această configurație creează o topologie de rețea rețea ce acceptă reproducerea directoarelor. O rețea virtuală poate acceptă mai multe seturi de reproducere, cu condiția ca fiecare set de reproducere să se află într-o subrețea virtuală diferită.

Pentru mai multe detalii despre setul de reproducere, consultați [Seturi de reproducere a conceptelor](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
