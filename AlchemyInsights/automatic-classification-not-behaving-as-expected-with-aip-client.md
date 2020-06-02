---
title: Clasificarea automată nu se comportă conform așteptărilor cu clientul AIP
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508388"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Clasificarea automată nu se comportă conform așteptărilor cu clientul AIP

Clasificarea automată nu se comportă conform așteptărilor, utilizați următoarele instrucțiuni recomandate:

1. Dacă aveți probleme cu etichetarea automată, consultați [Cum se configurează condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) și Ce caută tipurile de informații [sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Verificați dacă utilizați politici de domeniu care nu sunt configurate corect: [Cum se configurează politica azure protecția informațiilor pentru anumiți utilizatori utilizând politici ledomeniu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Dacă etichetarea automată nu funcționează pentru Outlook atunci când atașați un document etichetat, verificați că `DRMEncryptProperty` nu este definit ă ca descris ă aici: Setările de registry [IRM pentru securitate](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Dacă ați utilizat [tipurile de informații predefinite](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) pentru politica de protecție a informațiilor Azure, verificați dacă conținutul se potrivește cu formatul așteptat.
5. Verificați dacă eticheta este configurată corespunzător pentru **Automat** sau **Recomandat**. (Etichetarea automată este**disponibilă** pentru toate aplicațiile Office, în timp ce **recomandat** este disponibil pentru toate aplicațiile Office, cu excepția Outlook.)
6. Nu puteți utiliza clasificarea automată pentru documente și e-mailuri care au fost etichetate anterior manual sau etichetate anterior automat cu o clasificare mai mare.  Pentru mai multe informații, consultați: [Cum se aplică etichetele automate sau recomandate](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Dacă vă confruntați în continuare probleme, vă rugăm să colecteze Jurnalele de client Azure Information Protection și atașați jurnalele exportate la biletul de asistență. Pentru a exporta jurnalele azure informații de protecție:
    - Deschideți un document Office sau creați un e-mail nou în Outlook.
    - Faceți clic pe Ajutor și feedback **pentru protecție/sensibilitate**  >  **Help and feedback**.
    - Faceți clic pe **Export jurnale**.
    - Salvați jurnalele la alegerea locației și atașați-le la solicitarea de serviciu.

Pentru informații suplimentare, consultați:

- [se configurează condițiile pentru clasificarea automată și recomandată pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Ghiduri de utilizare pentru scenarii comune care utilizează Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Examinați documentația Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Revizuirea abonamentelor și caracteristicilor Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Cerințe pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tutorial de pornire rapidă pentru Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Descărcați clientul Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
