---
title: Depanarea accesului refuzat mesaje la OneDrive pentru site-uri business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511196"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Depanarea accesului refuzat mesaje la OneDrive pentru site-uri business

Această problemă apare cel mai frecvent atunci când un utilizator este șters și recreat cu același nume principal de utilizator (UPN). Noul cont este creat utilizând o valoare PUID (Passport Unique ID) diferită. Când utilizatorul încearcă să acceseze o colecție de site-ul sau OneDrive lor, utilizatorul are un PUID incorecte. Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint, și apoi sunt mutate într-un alt OU și resynced cu SharePoint, acestea pot apărea această problemă.

1. Pentru a rezolva această problemă ar trebui să restaurați UPN original cu pașii din articol, [Restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Dacă nu se poate restaura utilizatorul original ar trebui să eliminați utilizatorul vechi de pe site-ul OneDrive utilizând acești pași, [Eliminați un utilizator din lista de informații de utilizator](). 
3. După aceasta se face, puteți verifica utilizatorul are drepturi de administrator pe site-ul OneDrive urmând pașii pentru a [adăuga admin pentru OneDrive unui utilizator](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Pentru mai multe informații despre nivelurile de permisiune, consultați articolul, [Înțelegerea nivelurilor de permisiune în SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
