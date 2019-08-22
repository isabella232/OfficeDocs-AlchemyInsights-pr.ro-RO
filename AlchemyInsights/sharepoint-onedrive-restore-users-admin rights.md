---
title: Depanare acces refuzat mesaje OneDrive pentru afaceri site-uri
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507823"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Depanare acces refuzat mesaje OneDrive pentru afaceri site-uri

Această problemă apare cel mai frecvent atunci când un utilizator este şters şi re-creat cu acelaşi nume principal de utilizator (UPN). Noul cont este creat folosind o valoare diferită de PUID (paşaport unic ID). Atunci când utilizatorul încearcă să acceseze o colecţie de site-ul sau lor OneDrive, utilizatorul are un PUID incorecte. Un al doilea scenariu implică sincronizare director cu o unitate organizaţională de Active Directory (OU). În cazul în care utilizatorii au deja conectat la SharePoint, apoi sa mutat la un OU diferite şi resynced cu SharePoint, acestea se pot confrunta aceasta problema.

1. Pentru a rezolva această problemă, ar trebui să restabiliţi UPN original cu paşii din articol,[restaura un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. În cazul în care nu se poate restabili original utilizator ar trebui să eliminaţi utilizatorul vechi din site-ul OneDrive folosind aceşti paşi, [elimina un utilizator din lista de informaţii utilizator](). 
3. După ce acest lucru este făcut, puteţi verifica dacă utilizatorul are drepturi de administrator la site-ul OneDrive urmând paşii să [adăugaţi admin pe pentru un utilizator OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Pentru mai multe informaţii despre nivelurile de permisiune, a se vedea articolul, [nivelurile de permisiune de înţelegere în SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
