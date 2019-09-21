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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068035"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Jurnalele de audit SharePoint și OneDrive

**SharePoint și OneDrive modern audit Unified jurnalele de conformitate**

- [Activați/dezactivați înregistrarea în jurnal a auditului unificat](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nu este necesară nicio configurație suplimentară în SharePoint sau OneDrive.

- Utilizați căutarea în jurnal de audit pentru a verifica activitatea fișierului (fișierelor), folderului (ilor), utilizatorilor, permisiunilor:

    - [Activități de fișier și de pagini](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Activități folder](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Activități de partajare și acces la solicitări](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Activități de sincronizare](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Activitati de administrare a site-ului](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Pentru mai multe informații despre se recuperează aceste evenimente, consultați [Căutați Jurnalul de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Jurnalele de audit clasic SharePoint**

Am migrat SPO moștenire de audit pentru Unified audit log (UAL). Aceasta înseamnă, în esență, că toate rapoartele de audit moștenite SPO vor fi acum alimentate prin UAL, iar semnalele de audit moștenite au fost migrate la UAL.

Modificări cheie:

- Tundere ca o capacitate nu este disponibil.
- Secțiunea în care alegeți evenimente specifice pentru audit nu este disponibilă. Vă rugăm să consultați [acest document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod prestabilit.
- Opțiunea "locație" sub **rapoarte PARTICULARIZATE** nu este disponibilă. 
- Evenimentele "deschiderea sau descărcarea documentelor" nu sunt disponibile. 

