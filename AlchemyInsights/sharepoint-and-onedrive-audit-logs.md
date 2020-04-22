---
title: Rapoarte de jurnal de audit Are A fi audiate SharePoint clasice
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741977"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Jurnalele de audit SharePoint și OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Jurnalele de audit clasic SharePoint

Auditul moștenit spo a fost migrat în Jurnalul de audit unificat (UAL). Toate rapoartele de audit moștenite SPO vor fi alimentate acum prin UAL, iar semnalele de audit moștenite au fost migrate la UAL.

Modificări cheie:

* Tunderea NU este disponibilă ca o capacitate.
* Alegerea evenimentelor specifice pentru audit NU este disponibilă. Consultați [acest document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod implicit.
* Opțiunea **Locație** sub **Rapoarte personalizate** NU este disponibilă.
* Opțiunea **Deschiderea sau descărcarea evenimentelor de documente** NU este disponibilă.

[Configurarea setărilor de audit pentru o colecție de site-uri](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Jurnalele de audit unificat emititație SharePoint și OneDrive Modern Unified Audit din conformitate

* [Activarea/dezactivarea înregistrării în jurnal unificate a auditului](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Nu este necesară o configurație suplimentară în SharePoint sau OneDrive.

Utilizați căutarea în jurnal de auditare pentru a verifica activitatea fișierelor, folderelor, utilizatorului (utilizatorilor), permisiunilor:

* [Activități de fișiere și pagini](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Activități de foldere](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Partajarea și activitățile de solicitare a accesului](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Activități de sincronizare](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activități de administrare a sitului](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Pentru mai multe informații despre să regăsiți aceste evenimente, consultați [Căutarea în jurnalul de audit](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
