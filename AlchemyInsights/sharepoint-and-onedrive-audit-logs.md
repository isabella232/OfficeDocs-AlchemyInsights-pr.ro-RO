---
title: Rapoarte de jurnal de audit SharePoint clasic
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992630"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Jurnalele de audit SharePoint și OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Jurnalele de audit clasic SharePoint

Audit moștenire SPO a fost migrat la Unified audit log (UAL). Toate rapoartele de audit moștenite SPO vor fi acum alimentate prin UAL, iar semnalele de audit moștenite au fost migrate la UAL.

Modificări cheie:

* Tundere nu este disponibil ca o capacitate.
* Alegerea evenimentelor specifice pentru audit nu este disponibilă. Consultați [acest document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod implicit.
* Opțiunea de **locație** sub **rapoarte particularizate** nu este disponibilă.
* Opțiunea de **Deschidere sau descărcare documente** de evenimente nu este disponibilă.

[Configurați setările de audit pentru o colecție de site-uri](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint și OneDrive modern audit Unified jurnalele de conformitate

* [Activați/dezactivați înregistrarea în jurnal a auditului unificat](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nu este necesară nicio configurație suplimentară în SharePoint sau OneDrive.

Utilizați căutarea în jurnal de audit pentru a verifica activitatea fișierului (fișierelor), folderului (ilor), utilizatorilor, permisiunilor:

* [Activități de fișier și de pagini](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Activități folder](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Activități de partajare și acces la solicitări](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Activități de sincronizare](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activitati de administrare a site-ului](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Pentru mai multe informații despre se recuperează aceste evenimente, consultați [Căutați Jurnalul de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
