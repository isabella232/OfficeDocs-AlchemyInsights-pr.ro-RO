---
title: Crearea unui site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806951"
---
# <a name="create-a-sharepoint-site"></a>Crearea unui site SharePoint

Creați sau gestionați site-uri de la [site-uri active](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) în centrul de administrare SharePoint. Pentru mai multe informații, consultați [gestionarea site-urilor din noul centru de administrare SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation). 

## <a name="tips"></a>Sfaturi

- **Nu** puteți crea un site cu aceeași adresă URL a unui site existent. Dacă ați șters un site și doriți să reutilizați URL-ul, este posibil ca site-ul șters să existe încă sub [site-uri șterse](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true). Site-ul va trebui să fie șters definitiv pentru a reutiliza adresa URL. Pentru a elimina complet un site cu PowerShell, consultați exemplul cmdletului [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .
- Este posibil ca unii utilizatori să nu poată crea un site. [Consultați Gestionarea creării site-urilor în SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).
- Este posibil ca site-ul să apară blocat la **crearea** mai lungă decât cea așteptată. Dacă au trecut mai mult de 24 de ore de când ați văzut prima dată această problemă, vă rugăm să înregistrați un tichet de asistență. În multe cazuri, lucrăm deja la o soluție. Vă rugăm să ne dați cel puțin 24 de ore pentru a finaliza o soluție.
