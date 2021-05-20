---
title: 2681 Attack Liga în Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545738"
---
# <a name="attack-simulator-in-microsoft-365"></a>Atac Arădoare în Microsoft 365

- Ratați Atac 365? Attack Attack requires **Microsoft Defender for Office 365 Plan 2** or Office 365 Enterprise **E5.** Liga nu este **inclus** în Microsoft Defender pentru Office 365 Plan 1, Office 365 Enterprise E3 sau în Aplicații Microsoft 365 pentru afaceri abonamente.

- Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificare multi-factor (MFA). Pentru mai multe informații despre cerințele pentru atacurile din sua, [consultați acest articol.](/microsoft-365/security/office-365-security/attack-simulator)

- Aspecte importante de știt despre **simularea atacurilor** de tip Forță brută a parolelor:

  - În cazul în care contul țintă are activată autentificarea MFA și parola a fost ghicită corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).

  - Fișierul parolă nu poate fi mai mare de 10 MB. Utilizați o parolă pentru fiecare linie și includeți o linie necompletată (returnare linie) după ultima parolă din listă.

- Aspecte importante de spus despre **simularea atașării de phishing:**

  - Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul de server de conectare la phishing.**

  - Dacă un destinatar [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) utilizează programul de completare Activare mesaj raport pentru a raporta mesajul ca phishing, este posibil să nu primiți avertizări pentru mesaj (deoarece este un atac simulat).

- Rapoarte: După terminarea atacului simulat, puteți face clic pe Detalii **atac** pentru a vedea raportul.

- Pentru instrucțiuni detaliate și caracteristici noi în Atac 2010, [consultați Atac A se află în Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
