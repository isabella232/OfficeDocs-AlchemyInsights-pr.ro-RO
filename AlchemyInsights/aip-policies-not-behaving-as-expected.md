---
title: 'AIP: politicile nu se poartă așa cum vă așteptați'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663201"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politicile nu se poartă așa cum vă așteptați

Azure Information Protection: politicile care nu se poartă așa cum vă așteptați, consultați următoarele instrucțiuni pentru recomandările recomandate pentru diverse probleme de politică:

1. Dacă întâmpinați probleme cu marcajele vizuale, vă rugăm să revizuiți [atunci când se aplică marcaje vizuale](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Dacă întâmpinați probleme cu etichetarea automată, consultați [cum să configurați condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și [ce caută tipurile sensibile de informații](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Dacă întâmpinați probleme cu protecția nativ/Pfile, examinați [configurația API a fișierelor](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: [cum se configurează Politica de protecție a informațiilor Azure pentru anumiți utilizatori, utilizând politicile de domeniu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, Verificați dacă DRMEncryptProperty nu este definit așa cum este descris aici: [setările de registry IRM pentru securitate](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Dacă întâmpinați în continuare probleme, vă rugăm să colectați jurnalele clienților Azure Information Protection și să atașați jurnalele exportate la acest bilet.

1. Deschideți un document Office sau creați un mesaj de e-mail nou în Outlook.
2. Faceți clic pe **Protejare/sensibilitate**  >  **Ajutor și feedback**.
3. Faceți clic pe **Export jurnale**.
4. Salvați jurnalele la alegerea locației și atașați-le la această solicitare de serviciu.

Resurse suplimentare:

- [Cum se configurează o etichetă pentru marcaje vizuale pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Revizuirea documentației Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Utilizarea etichetelor de sensibilitate în aplicațiile Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

