---
title: Identifica adresa IP şi client în jurnalele de auditare
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539041"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifica adresa IP şi client în jurnalele de auditare

IP-ul care corespunde unei activități de către un utilizator Office 365 sau administratorul este indicat în jurnalele de Audit. Informaţii client este, de asemenea, conectat. Aici sunt paşii pentru astfel de informaţii de identificare

1. Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/).

2. Du-te la **Căutare** > pagina de**Căutare de jurnalul de Audit** .

   Dacă sunteţi interesat într-o activitate specifică, selectaţi-l din lista de **activităţi** . Dacă nu, toate activităţile vor fi returnate pentru utilizator selectat (setarea implicită).

   **Notă**: anumite activităţi să nu fie disponibilă în meniul de **activităţi** ; cu toate acestea, cei de audit elemente vor fi returnate dacă **Arată rezultate pentru toate acțiunile** este selectat (. lipsă aranjare).

3. Specificaţi numele de utilizator în câmpul **utilizatorilor** , selectaţi intervalul de date corespunzător pentru activitatea şi apoi faceţi clic pe **Căutare**.

În rezultate, puteţi vedea adresa IP pentru activitatea respectivă în panoul de rezultate. Selectaţi înregistrarea de audit pentru a vedea informaţii detaliate în fișă de **Detalii** (de exemplu, Client, utilizatorul care a efectuat acţiunea, etc.).

Pentru informaţii suplimentare, consultaţi [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromise](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
