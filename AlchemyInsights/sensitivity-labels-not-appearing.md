---
title: Etichetele de sensibilitate nu apar
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801196"
---
# <a name="sensitivity-labels-not-appearing"></a>Etichetele de sensibilitate nu apar

Etichetele de sensibilitate vă permit să clasificați și să contribuiți la protejarea conținutului sensibil. Acestea pot fi create în centrul de conformitate Microsoft 365, centrul de securitate Microsoft 365 sau în centrul de conformitate Microsoft 365 Security & conform clasificării > etichetele de sensibilitate. Pentru a afla mai multe despre această caracteristică, consultați [prezentarea generală a etichetelor de sensibilitate](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Dacă ați configurat etichetele de sensibilitate, dar acestea nu apar în aplicațiile Microsoft 365, verificați următoarele:

- Confirmați că eticheta de sensibilitate a fost [publicată](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) utilizatorilor și grupurilor dorite.

- Confirmați că utilizatorul utilizează o aplicație care acceptă etichetele de sensibilitate-vedeți [etichetele de sensibilitate în document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Dacă [migrați etichetele Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), țineți cont de considerațiile listate [aici](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Suport pentru prevenirea pierderii datelor (DLP): în prezent, numai etichetele de retenție pot fi utilizate ca o condiție în politicile DLP.  Asistența pentru etichetele de sensibilitate dintr-o politică DLP nu este disponibilă încă, dar lucrăm la aceasta.

- Atunci când criptarea este activată pe o etichetă de sensibilitate, puteți alege una dintre următoarele:
    - Atribuirea permisiunilor acum
    - Permiteți utilizatorilor să atribuie permisiuni


Pentru mai multe informații despre problemele posibile, consultați [probleme cunoscute cu etichetele de sensibilitate](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).