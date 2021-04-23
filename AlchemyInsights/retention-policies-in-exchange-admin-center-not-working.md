---
title: Politicile de retenție din Centrul de administrare Exchange nu funcționează
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952240"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politicile de retenție în Centrul de administrare Exchange

Dacă doriți să rulam verificări automate pentru setările menționate mai jos, selectați butonul Înapoi < - în partea de sus a acestei pagini, apoi introduceți adresa de e-mail a utilizatorului care are probleme cu politicile de retenție.

Dacă aveți probleme cu politicile de conservare din Centrul de administrare Exchange care nu se aplică la cutiile poștale sau elementele care nu se mută în cutia poștală de arhivare, verificați următoarele:

**Cauze rădăcină:**

- **Asistentul de foldere gestionate** nu a procesat cutia poștală a utilizatorului. Asistentul de foldere gestionate încearcă să proceseze fiecare cutie poștală din organizația dvs. bazată pe cloud o dată la șapte zile.

  **Soluție:** Rulați Asistentul de foldere gestionate.

- **Reținerea a** fost **activată pentru cutia** poștală. Dacă cutia poștală a fost plasată pe o Reținere de retenție, politica de reținere pentru cutia poștală nu va fi procesată în acest timp.

  **Soluție:** Verificați starea setării Reținere în așteptare și actualizați după cum este necesar. Pentru detalii, consultați Reținerea în așteptare [a cutiei poștale.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Notă:** Dacă o cutie poștală este mai mică de 10 MB, Asistentul de foldere gestionate nu va procesa automat cutia poștală.
 
Pentru mai multe informații despre politicile de retenție din Centrul de administrare Exchange, consultați:

- [Etichetele de retenție și politicile de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Aplicarea unei politici de retenție pentru cutiile poștale sau](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Adăugarea sau eliminarea etichetelor de retenție](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Cum să identificați tipul de așteptare plasat pe o cutie poștală](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
