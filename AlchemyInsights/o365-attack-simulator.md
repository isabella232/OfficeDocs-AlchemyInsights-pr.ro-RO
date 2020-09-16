---
title: 2681 Attack Simulator în Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759231"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulatorul de atac în Microsoft 365

- Vă lipsește simulatorul de atacuri? Simulatorul de atacuri necesită **office 365 Advanced Threat Protection Plan 2 (ATP plan 2)** sau **Office 365 Enterprise E5**. Simulatorul de atacuri **nu** este inclus în Office 365 Advanced Threat Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3 sau orice aplicații Microsoft 365 pentru firme pentru abonamente.

- Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni de administrator global sau de administrator de securitate și autentificarea multi-factor (AMF). Pentru mai multe informații despre cerințele pentru simulatorul de atacuri, consultați [acest subiect](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Lucruri importante de știut despre simulările de atacuri cu **parolă brută Force** :

  - Dacă contul țintă are AMF activat și parola a fost ghicit corect, contul nu se va afișa ca compromis (al doilea factor de autentificare va fi incomplet).

  - Fișierul parolă nu poate fi mai mare de 10 MO. Utilizați o parolă per linie și includeți o linie necompletată (retur transport) după ultima parolă din listă.

- Lucruri importante de știut despre simulările de **înșelătorie** atașate de Lance:

  - Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul serverului de conectare la phishing**.

  - Dacă un destinatar utilizează programul de [completare activare mesaj raport](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pentru a raporta mesajul ca phishing, este posibil să nu primiți avertizări pentru mesaj (deoarece acesta este un atac simulat).

- Rapoarte: după finalizarea atacului simulat, puteți să faceți clic pe **Detalii despre atacuri** pentru a vedea raportul.

- Pentru instrucțiuni detaliate și caracteristici noi în simulatorul de atacuri, consultați [Attack Simulator în Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
