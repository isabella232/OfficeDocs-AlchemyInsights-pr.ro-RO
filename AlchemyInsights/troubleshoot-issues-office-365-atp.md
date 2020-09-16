---
title: Depanarea problemelor cu Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758077"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Depanarea problemelor cu Office 365 ATP

- **Observați întârzieri cu livrarea mesajelor de e-mail**? Încercați să utilizați opțiunea de livrare dinamică pentru politicile de atașări sigure pentru ATP. Acest lucru va evita întârzierile livrării mesajelor de e-mail în timp ce protejează destinatarii din fișiere rău intenționate.
- **Doriți să raportați pozitive false sau negative false**? Utilizați acest link pentru a trimite fișierul pentru analiză: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Știați că puteți permite protecția linkurilor de siguranță ATP pentru mesajele de e-mail trimise între persoanele din organizația dvs**.? Urmați acești pași:
    1. Accesați https://protection.office.com și conectați-vă.
    2. Accesați **Threat management**  >  **Policy**  >  **linkuri sigure**pentru Politica de gestionare a amenințărilor.
    3. Sub **politici care se aplică pentru anumiți destinatari**, editați (sau adăugați) o politică.
    4. Selectați **se aplică Linkuri sigure la mesajele trimise în cadrul Organizației**.
    5. Salvați politica și permiteți aproximativ 30 de minute pentru ca modificările să funcționeze în centrul de date.
- Pentru a obține mai mult ajutor pentru ATP, consultați [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).