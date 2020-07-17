---
title: 'AIP: Politicile nu se comportă conform așteptărilor'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506570"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politicile nu se comportă conform așteptărilor

Azure informații protecția: Politicile nu se comportă conform așteptărilor, consultați următoarele pentru liniile directoare recomandate pentru diverse probleme de politică:

1. Dacă aveți probleme cu marcajele vizuale, vă rugăm să examinați [Când se aplică marcajele vizuale](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Dacă aveți probleme cu etichetarea automată, consultați [Cum se configurează condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Dacă aveți probleme cu protecția native / Pfile, vă rugăm să revizuiți [configurația File API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: [Cum se configurează politica azure protecția informațiilor pentru anumiți utilizatori utilizând politici ledomeniu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, verificați dacă DRMEncryptProperty nu este definit așa este descris aici: [Setările de registry IRM pentru securitate](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Dacă vă confruntați în continuare probleme, vă rugăm să colecteze Jurnalele de client Azure Information Protection și atașați jurnalele exportate la acest bilet.

1. Deschideți un document Office sau creați un e-mail nou în Outlook.
2. Faceți clic pe Ajutor și feedback **pentru protecție/sensibilitate**  >  **Help and feedback**.
3. Faceți clic pe **Export jurnale**.
4. Salvați jurnalele la alegerea locației și atașați-le la această solicitare de serviciu.

Resurse suplimentare:

- [se configurează o etichetă pentru marcaje vizuale pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Examinați documentația Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Utilizarea etichetelor de sensibilitate în aplicațiile Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

