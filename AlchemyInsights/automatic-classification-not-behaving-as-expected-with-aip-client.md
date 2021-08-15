---
title: Clasificarea automată nu are loc așa cum este așteptat cu clientul AIP
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979721"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Clasificarea automată nu are loc așa cum este așteptat cu clientul AIP

Clasificarea automată nu are rezultatele așteptate, utilizați următoarele instrucțiuni recomandate:

1. Dacă aveți probleme cu etichetarea automată, consultați Cum se configurează condițiile pentru clasificarea automată și recomandată pentru [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și Ce tipuri de informații sensibile [caută.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: Cum se configurează politica [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)pentru utilizatori specifici utilizând politici de domeniu.
3. Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, verificați dacă nu este definită după cum este descris aici: Setări de `DRMEncryptProperty` [registry IRM pentru securitate.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Dacă ai utilizat [tipurile de informații predefinite pentru](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) politica Azure Information Protection, verificați dacă conținutul se potrivește cu formatul așteptat.
5. Verificați dacă eticheta este configurată corespunzător pentru **Automat** sau **Recomandat.** (**Etichetarea** automată este disponibilă pentru toate  aplicațiile Microsoft 365, în timp ce Recomandare este disponibilă pentru toate aplicațiile Microsoft 365, cu excepția Outlook.)
6. Nu puteți utiliza clasificarea automată pentru documente și mesaje de e-mail care au fost etichetate anterior manual sau etichetate anterior cu o clasificare superioară.  Pentru mai multe informații, consultați: [Cum se aplică etichetele automate sau recomandate.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Dacă încă aveți probleme, colectați jurnale ale clientului Azure Information Protection și atașați jurnalele exportate la tichetul de asistență. Pentru a exporta jurnalele Azure Information Protection:
    - Deschideți un document Office sau creați un mesaj de e-mail nou în Outlook.
    - Faceți clic pe Ajutor și feedback **pentru**  >  **protejare/sensibilitate.**
    - Faceți **clic pe Export jurnale.**
    - Salvați jurnalele la alegerea locației și atașați-le la solicitarea de serviciu.

Pentru informații suplimentare, consultați:

- [Cum se configurează condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Ghiduri detaliate pentru scenarii comune care utilizează Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Revizuiți documentația Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Revizuiți abonamentele și caracteristicile Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Cerințe pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tutorial de pornire rapidă pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Descărcați clientul Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
