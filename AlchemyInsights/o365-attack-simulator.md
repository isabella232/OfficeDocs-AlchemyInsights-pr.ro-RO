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
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895803"
---
# <a name="attack-simulator-in-microsoft-365"></a>Atac Arădoare în Microsoft 365

- Ratați Atac 365? Pentru A4, **Microsoft Defender necesită Microsoft Defender Office 365 Plan 2** sau Office 365 Enterprise **E5.** Liga nu este **inclus** în Microsoft Defender pentru Office 365 Plan 1, Office 365 Enterprise E3 sau în Aplicații Microsoft 365 pentru afaceri abonamente.

- Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificare multi-factor (MFA). Pentru mai multe informații despre cerințele pentru atacurile din sua, [consultați acest articol.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Aspecte importante de știt despre **simularea atacurilor** de tip Forță brută a parolelor:

  - În cazul în care contul țintă are activată autentificarea MFA și parola a fost ghicită corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).

  - Fișierul parolă nu poate fi mai mare de 10 MB. Utilizați o parolă pentru fiecare linie și includeți o linie necompletată (returnare linie) după ultima parolă din listă.

- Aspecte importante de spus despre **simularea atașării de phishing:**

  - Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul de server de conectare la phishing.**

  - Dacă un destinatar [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) utilizează programul de completare Activare mesaj raport pentru a raporta mesajul ca phishing, este posibil să nu primiți avertizări pentru mesaj (deoarece este un atac simulat).

- Rapoarte: După terminarea atacului simulat, puteți face clic pe Detalii **atac** pentru a vedea raportul.

- Pentru instrucțiuni detaliate și caracteristici noi în Atac 365, [consultați Atac Sau în Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
