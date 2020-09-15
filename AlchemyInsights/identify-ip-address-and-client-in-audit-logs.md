---
title: Identificarea adresei IP și a clientului în jurnalele de auditare
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668322"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificarea adresei IP și a clientului în jurnalele de auditare

Adresa IP care corespunde unei activități de către un utilizator sau administrator Microsoft 365 este afișată în jurnalele de auditare. Informațiile clientului sunt, de asemenea, înregistrate. Iată pașii pentru identificarea acestor informații

1. Conectați-vă la [Centrul de conformitate Microsoft 365 Security &](https://protection.office.com/).

2. Accesați **Search**  >  pagina**Căutare în Jurnalul de auditare** căutare.

   Dacă sunteți interesat de o anumită activitate, selectați-o din lista de **activități** . Dacă nu, toate activitățile vor fi returnate pentru utilizatorul selectat (setarea implicită).

   **Notă**: este posibil ca anumite activități să nu fie disponibile în meniul **activități** ; cu toate acestea, acele elemente de audit vor fi returnate dacă se selectează **Afișare rezultate pentru toate activitățile** (setare implicită).

3. Specificați numele de utilizator în câmpul **utilizatori** , selectați intervalul de date corespunzător pentru activitate, apoi faceți clic pe **Căutare**.

În rezultate, puteți vedea adresa IP pentru acea activitate în panoul rezultate. Selectați înregistrarea de audit pentru a vedea informații detaliate în **detaliile** flyout (de exemplu, client, utilizator care a efectuat acțiunea etc.).

Pentru mai multe informații, consultați [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromis](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
