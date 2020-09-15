---
title: Rapoarte jurnal de audit SharePoint clasic
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662220"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Jurnalele de audit SharePoint și OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Jurnalele de audit SharePoint Classic

Auditarea moștenită SPO a fost migrată în jurnal de audit unificat (nepotrivit). Toate rapoartele de audit moștenite de la SPO vor fi alimentate acum prin intermediul, iar semnalele de audit moștenite au fost migrate la un raport.

Modificări cheie:

* Tunderea nu este disponibilă ca o capacitate.
* Nu este disponibilă alegerea anumitor evenimente de auditare. Consultați [acest document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) pentru o listă completă a evenimentelor auditate disponibile în mod implicit.
* Opțiunea **locație** de sub **rapoarte particularizate** nu este disponibilă.
* Opțiunea **Deschidere sau descărcare documente** evenimente nu este disponibilă.

[Configurarea setărilor de audit pentru o colecție de site-uri](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Jurnalele de audit unificate moderne SharePoint și OneDrive de la conformitate

* [Activarea/dezactivarea înregistrării în jurnal a auditării unificate](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Nu este necesară nicio configurare suplimentară în SharePoint sau OneDrive.

Utilizarea căutării în înregistrarea în jurnal a auditării pentru a verifica activitatea fișierelor, a folderelor, a utilizatorilor, a permisiunilor:

* [Activități de fișier și de pagină](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Activități de foldere](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Activități de partajare și de solicitare a accesului](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Activități de sincronizare](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activități de administrare a site-ului](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Pentru mai multe informații despre cum să regăsiți aceste evenimente, consultați [căutarea în Jurnalul de auditare](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
