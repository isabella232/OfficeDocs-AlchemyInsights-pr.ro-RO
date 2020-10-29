---
title: Depanarea problemelor cu Microsoft Defender pentru Office 365 (ATP)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801419"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Depanarea problemelor cu Office 365 ATP

- **Observați întârzieri cu livrarea mesajelor de e-mail** ? Încercați să utilizați opțiunea de livrare dinamică pentru politicile de atașări sigure pentru ATP. Acest lucru va evita întârzierile livrării mesajelor de e-mail în timp ce protejează destinatarii din fișiere rău intenționate.
- **Doriți să raportați pozitive false sau negative false** ? Utilizați acest link pentru a trimite fișierul pentru analiză: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Știați că puteți permite protecția linkurilor de siguranță ATP pentru mesajele de e-mail trimise între persoanele din organizația dvs** .? Urmați acești pași:
    1. Accesați https://protection.office.com și conectați-vă.
    2. Accesați **Threat management**  >  **Policy**  >  **linkuri sigure** pentru Politica de gestionare a amenințărilor.
    3. Sub **politici care se aplică pentru anumiți destinatari** , editați (sau adăugați) o politică.
    4. Selectați **se aplică Linkuri sigure la mesajele trimise în cadrul Organizației** .
    5. Salvați politica și permiteți aproximativ 30 de minute pentru ca modificările să funcționeze în centrul de date.
- Pentru a obține mai mult ajutor pentru ATP, consultați [Microsoft Defender pentru Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).