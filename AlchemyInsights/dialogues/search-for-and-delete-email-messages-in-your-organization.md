---
title: Căutarea și ștergerea mesajelor de e-mail din organizație
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525439"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Căutarea și ștergerea mesajelor de e-mail din organizație

Urmați acești pași:

1. Dacă nu sunteți administrator global, pentru a căuta mesaje, contul trebuie adăugat la **grupul de roluri EDiscovery Manager** sau la rolul de **gestionare a căutării conformității**. Pentru a șterge mesaje, va trebui să vă asociați **grupului de roluri pentru gestionarea organizației** sau **rolul de gestionare a căutării și eliminării**. Permisiunile pentru aceste roluri sunt atribuite în [Centrul de securitate & conformitate.](https://protection.office.com)
2. [Creați o căutare de conținut](https://docs.microsoft.com/office365/securitycompliance/content-search) pentru a găsi mesajul de șters.
3. [Conectați-vă la Security & Conformity Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Dacă utilizați Mae, consultați aceste instrucțiuni: [conectarea la Security & la centrul de conformitate PowerShell utilizând autentificarea multi-factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Ștergeți mesajul: rulează `New-ComplianceSearchAction` cmdletul pentru a șterge mesajul. Mesajele șterse sunt mutate în folderul Elemente recuperabile ale unui utilizator. Pentru o comandă exemplu, consultați [Pasul 3: ștergerea mesajului.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
