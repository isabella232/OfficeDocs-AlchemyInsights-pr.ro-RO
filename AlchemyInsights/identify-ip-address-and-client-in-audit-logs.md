---
title: Identificarea adresei IP și a clientului în jurnalele de audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716400"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificarea adresei IP și a clientului în jurnalele de audit

Adresa IP care corespunde unei activități de către un utilizator sau administrator Microsoft 365 este afișată în Jurnalele de audit. Informațiile despre client sunt, de asemenea, înregistrate. Iată pașii pentru identificarea acestor informații

1. Conectați-vă la Centrul de [conformitate Microsoft 365 Security &](https://protection.office.com/).

2. Accesați pagina de căutare în jurnalul **De** > **audit căutare.**

   Dacă sunteți interesat de o anumită activitate, selectați-o din lista **Activități.** Dacă nu, toate activitățile vor fi returnate pentru utilizatorul selectat (setare implicită).

   **Notă:** Este posibil ca anumite activități să nu fie disponibile în meniul **Activități;** cu toate acestea, aceste elemente de audit vor fi returnate dacă **se afișează rezultate pentru toate activitățile** este selectat (setareimplicită).

3. Specificați numele de utilizator în câmpul **Utilizatori,** selectați intervalul de date corespunzător pentru activitate, apoi faceți clic pe **Căutare**.

În rezultate, puteți vedea adresa IP pentru acea activitate în panoul de rezultate. Selectați înregistrarea de audit pentru a vedea informații detaliate în ieșirea **Detalii** (de exemplu, Client, Utilizator care a efectuat acțiunea etc.).

Pentru mai multe informații, consultați [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromis](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
