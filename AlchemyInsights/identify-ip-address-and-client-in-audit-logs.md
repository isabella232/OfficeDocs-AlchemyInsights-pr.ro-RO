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
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382965"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifica adresa IP şi client în jurnalele de auditare

IP-ul care corespunde unei activități de către un utilizator sau administrator este indicat în jurnalele de Audit. Informaţii client este, de asemenea, conectat. Aici sunt paşii pentru astfel de informaţii de identificare

1. Conectaţi-vă la [Centrul de conformitatea Office 365 securitate &](https://protection.office.com/)

2. Faceţi clic pe **Căutare şi ancheta** şi selectaţi **Căutare de jurnalul de Audit**.

   Dacă sunteţi interesat într-o activitate specifică, selectaţi-l din lista de **activităţi** . Dacă nu, toate activităţile vor fi returnate pentru utilizator selectat (setarea implicită).

   **Notă**: anumite activităţi să nu fie disponibilă în meniul de **activităţi** ; cu toate acestea, cei de audit elemente vor fi returnate dacă **Arată rezultate pentru toate acțiunile** este selectat (. lipsă aranjare).

3. Specificaţi numele de utilizator în câmpul **utilizatorilor** , selectaţi intervalul de date corespunzător pentru activitatea şi apoi faceţi clic pe **Căutare**.

În rezultate, puteţi vedea adresa IP pentru activitatea respectivă în panoul de rezultate. Selectaţi înregistrarea de audit pentru a vedea informaţii detaliate în fișă de **Detalii** (de exemplu, Client, utilizatorul care a efectuat acţiunea, etc.).

Pentru informaţii suplimentare, consultaţi [Găsirea adresei IP a computerului utilizat pentru a accesa un cont compromise](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
