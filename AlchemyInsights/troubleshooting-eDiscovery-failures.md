---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105580"
---
# <a name="troubleshoot-content-search-errors"></a>Depanarea erorilor de căutare de conținut

Aveți probleme cu Căutarea conținutului sau obțineți erori atunci când exportați rezultatele căutării?

De exemplu, primiți următoarele atunci când rulați căutări?

- Erori CS008 sau CS012

- Erori de ocupat/expirare server

- S-a produs o eroare la aplicație

Sau atunci când căutați sau exportați rezultate dintr-un număr mare de cutii poștale (peste 100.000 de cutii poștale), obțineți erori de export?

Pentru aceste tipuri de erori, reîncercați să căutați locațiile de conținut care nu au reușit. Consultați  [acest articol](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) pentru mai multe informații.

Dacă exportați mai mult de 100.000 de cutii poștale, va trebui să utilizați următorul Powershell pentru a descărca rezultatele exportului: exportul rezultatelor din peste  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)de cutii poștale.
