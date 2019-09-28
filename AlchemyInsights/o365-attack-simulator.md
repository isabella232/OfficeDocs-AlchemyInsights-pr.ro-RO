---
title: 2681 Simulator de atac în Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305343"
---
# <a name="attack-simulator-in-office-365"></a>Simulator de atac în Office 365

- Iti lipseste Attack Simulator? Simulator de atac necesită **Office 365 Advanced amenințare Protection Plan 2 (ATP plan 2)** sau **Office 365 Enterprise E5**. Attack Simulator **nu** este inclus în Office 365 Advanced amenințare Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3, sau orice Office 365 Business abonamente.

- Contul pe care îl utilizați pentru a lansa atacuri simulate necesită permisiuni globale de administrator sau administrator de securitate și autentificarea multi-factor (MFA). Pentru mai multe informații despre cerințele de atac Simulator, consultați [acest subiect](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Lucruri importante să știți despre **brute force parola** atac simulări:

  - Dacă contul țintă are MFA activat și parola a fost ghicit corect, contul nu va afișa ca compromis (al doilea factor de autentificare va fi incomplet).

  - Fișierul de parolă nu poate fi mai mare de 10 MB. Utilizați o parolă pe linie și includeți o linie necompletată (retur transport) după ultima parolă din listă.

- Lucruri importante de știut despre **suliță phishing** atașați simulări:

  - Prin proiectare, nu puteți furniza o valoare particularizată pentru **URL-ul serverului de conectare la phishing**.

  - Dacă un destinatar utilizează [permite Add-in raport mesaj](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) pentru a raporta mesajul ca phishing, este posibil să nu primiți alerte pentru mesaj (deoarece acesta este un atac simulat).

- Rapoarte: după terminarea atacului simulat, puteți face clic pe **Detalii atac** pentru a vedea raportul.

- Pentru instrucțiuni detaliate și caracteristici noi în Attack Simulator, consultați [Attack Simulator în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
