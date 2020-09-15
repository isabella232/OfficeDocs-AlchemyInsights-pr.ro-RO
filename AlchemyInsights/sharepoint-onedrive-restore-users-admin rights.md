---
title: Depanarea mesajelor refuzate pentru site-urile OneDrive pentru Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670628"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Depanarea mesajelor refuzate pentru site-urile OneDrive pentru Business

Această problemă apare cel mai frecvent atunci când un utilizator este șters și creat din nou cu același nume principal de utilizator (UPN). Noul cont este creat utilizând o altă valoare PUID (ID unic Passport). Atunci când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive, utilizatorul are o PUID incorectă. Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint, apoi sunt mutați la alt OU și Resincronizați cu SharePoint, este posibil ca aceștia să întâmpine această problemă.

1. Pentru a rezolva această problemă, trebuie să restaurați UPN-ul inițial cu pașii din articol, să [restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Dacă nu puteți restaura utilizatorul inițial, ar trebui să eliminați utilizatorul vechi din site-ul OneDrive utilizând acești pași, să [Eliminați un utilizator din lista informații utilizator](). 
3. După ce se termină acest lucru, puteți verifica dacă utilizatorul are drepturi de administrator la site-ul OneDrive, urmând pașii de [Adăugare a administratorului pentru OneDrive unui utilizator](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Pentru mai multe informații despre nivelurile de permisiune, consultați articolul, [înțelegerea nivelurilor de permisiune din SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
