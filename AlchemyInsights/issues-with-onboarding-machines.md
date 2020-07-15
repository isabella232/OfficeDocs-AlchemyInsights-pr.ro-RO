---
title: Probleme cu mașinile de îmbarcare
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141658"
---
# <a name="issues-with-onboarding-machines"></a>Probleme cu mașinile de îmbarcare

Este posibil să aveți probleme cu mașinile de îmbarcare pentru serviciul MDATP. Dacă puteți accesa computerul utilizatorului final, urmați acești pași:

1. Descărcați instrumentul de diagnosticare [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)
2. Extrageți și executați MDATPAnalyzer.cmd.
3. Găsiți jurnalul de diagnosticare în folderul numit MDATPClientAnalyzerResult, același folder în care este descărcat instrumentul Analyzer.
4. Examinați fișierul jurnal, MDATPClientAnalyzer.txt, pentru a găsi probleme de conectivitate sau setări proxy internet.