---
title: Importul și exportul din Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037261"
---
# <a name="import-and-export-from-yammer"></a>Importul și exportul din Yammer

**Importul**

Opțiunile de import pentru utilizatori variază în funcție de faptul dacă rețeaua Yammer este în [modul nativ pentru Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)sau nu.

- **Mod non-nativ**: utilizatorii pot fi importați în grupuri utilizând [Adăugare din agendă](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (se limitează la utilizatorii 100) din setările de grup sau din rețea, utilizând [actualizarea masivă](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) din administratorul de rețea.
- **Mod nativ**: apartenența la grup și operațiunile de apartenență la rețea ar trebui să fie efectuate de la [portalul de administrare Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)sau utilizând altă opțiune Azure AD. Rețelele din modul nativ nu mai au acces la actualizarea în masă și la alte caracteristici moștenite.

> [!IMPORTANT]
> Yammer nu a acceptat niciodată importul conținutului din interiorul administratorului de rețea chiar și atunci când s-a utilizat caracteristica Export date în altă rețea. Conținutul poate fi repostat de soluții pentru parteneri sau API-uri de REST Yammer.

**Export**

[Exportul datelor din rețea în cadrul administratorului de rețea](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permite exportul de conținut din rețelele Yammer, inclusiv mesaje și fișiere. Atașările pot fi extrem de mari și vor determina exportul să dureze un timp semnificativ. Vă recomandăm să exportați rețele active utilizând [API](https://developer.yammer.com/docs/data-export-api) -ul de export de date din bucăți după zi sau săptămână. Asistența Microsoft nu furnizează scripturi particularizate în acest scop.

Există un [Export RGPD](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) separat pentru exportul conținutului pentru un utilizator individual.