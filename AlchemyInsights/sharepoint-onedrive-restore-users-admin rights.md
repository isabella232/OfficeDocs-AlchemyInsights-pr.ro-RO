---
title: Depanarea accesului refuzat mesaje la OneDrive for Business site-uri
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766723"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Depanarea accesului refuzat mesaje la OneDrive for Business site-uri

Această problemă apare cel mai frecvent atunci când un utilizator este șters și re-creat cu același nume principal de utilizator (UPN). Noul cont este creat utilizând un alt PUID (pașaport Unique ID) valoare. Când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive lor, utilizatorul are un PUID incorect. Un al doilea scenariu implică sincronizare director cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint și apoi sunt mutate într-un ou diferit și traducerea cu SharePoint, acestea pot experimenta această problemă.

1. Pentru a rezolva această problemă ar trebui să restaurați UPN originală cu pașii din articol, [restaurați un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Dacă nu se poate restaura utilizatorul original ar trebui să eliminați utilizatorul vechi din site-ul OneDrive utilizând acești pași, [Eliminați un utilizator din lista de informații de utilizator](). 
3. După ce se face acest lucru, aveți posibilitatea să verificați că utilizatorul are drepturi de administrator la site-ul OneDrive urmând pașii pentru a [adăuga admin pentru un utilizator OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

Pentru mai multe informații despre nivelurile de permisiune, consultați articolul, [înțelegerea nivelurilor de permisiune în SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
