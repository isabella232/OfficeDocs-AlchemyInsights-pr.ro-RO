---
title: Depanarea Access - mesaje refuzate la site OneDrive pentru business uri
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957805"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Depanarea Access - mesaje refuzate la site OneDrive pentru business uri

Această problemă apare de cele mai multe ori când un utilizator este șters și creat din nou cu același nume principal de utilizator (UPN). Noul cont este creat utilizând o altă valoare PUID (Pașaport unic). Atunci când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive său, utilizatorul are un PUID incorect. Al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint, apoi sunt mutati la un alt OU și sunt resincroniți cu SharePoint, aceștia pot experimenta această problemă.

1. Pentru a rezolva această problemă, trebuie să restaurați UPN-ul original cu pașii din articol [Restaurarea unui utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Dacă nu puteți restaura utilizatorul original, trebuie să eliminați utilizatorul vechi din site-ul OneDrive utilizând acești pași, Eliminați un utilizator din lista [de informații despre utilizator.]() 
3. După ce se face aceasta, puteți verifica dacă utilizatorul are drepturi de administrator la site-ul OneDrive, urmând pașii pentru Adăugarea permisiunilor de [administrator pentru](https://docs.microsoft.com/sharepoint/manage-user-profiles) OneDrive

Pentru mai multe informații despre nivelurile de permisiune, consultați articolul Despre [nivelurile de permisiune din SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
