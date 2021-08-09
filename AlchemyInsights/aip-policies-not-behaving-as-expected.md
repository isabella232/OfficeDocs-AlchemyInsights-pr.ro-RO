---
title: 'AIP: Politicile nu se comportă așa cum vă așteptați'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934305"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politicile nu se comportă așa cum vă așteptați

Azure Information Protection: Politicile nu au un comportament așa cum vă așteptați, consultați următoarele pentru instrucțiuni recomandate pentru diverse probleme de politică:

1. Dacă aveți probleme cu marcajele vizuale, revizuiți [Atunci când se aplică marcaje vizuale.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Dacă aveți probleme cu etichetarea automată, revizuiți Cum se configurează condițiile pentru clasificarea automată și recomandată pentru [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și Ce tipuri de informații sensibile [caută.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Dacă aveți probleme cu protecția Native/Pfile, revizuiți [configurația FILE API.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: Cum se configurează politica [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)pentru utilizatori specifici utilizând politici de domeniu.
5. Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, verificați dacă DRMEncryptProperty nu este definit după cum este descris aici: Setări de [registry IRM pentru](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)securitate.

Dacă încă aveți probleme, colectați jurnale ale clientului Azure Information Protection și atașați jurnalele exportate la acest tichet.

1. Deschideți un document Office sau creați un mesaj de e-mail nou în Outlook.
2. Faceți clic pe Ajutor și feedback **pentru**  >  **protejare/sensibilitate.**
3. Faceți **clic pe Export jurnale.**
4. Salvați jurnalele la alegerea locației și atașați-le la această solicitare de serviciu.

Resurse suplimentare:

- [Cum se configurează o etichetă pentru marcajele vizuale pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Revizuiți documentația Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Utilizați etichete de sensibilitate în Microsoft 365 aplicații](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

