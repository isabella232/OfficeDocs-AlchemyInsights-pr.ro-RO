---
title: Depanarea mesajelor refuzate la acces
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758498"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Depanarea mesajelor refuzate de acces în Centrul de administrare Sharepoint/OneDrive

Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un Centru de administrare Sharepoint/OneDrive, asigurați-vă că [atribuiți o licență utilizatorului](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Dacă utilizatorul are o licență, trebuie să vă asigurați că li se [atribuie un rol de administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) care poate accesa centrele de administrare.

Această problemă poate apărea, de asemenea, atunci când un utilizator este șters și recreat cu același nume principal de utilizator (UPN). Noul cont este creat utilizând o valoare PUID (Passport Unique ID) diferită. Când utilizatorul încearcă să acceseze o colecție de site-ul sau OneDrive lor, utilizatorul are un PUID incorecte. Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint, și apoi sunt mutate într-un alt OU și resynced cu SharePoint, acestea pot apărea această problemă.

Pentru a rezolva această problemă, ar trebui să restaurați UPN original cu pașii din articol, [Restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Notă: Dacă un centru de administrare OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut anterior acces, este posibil să existe o problemă de serviciu temporar.  [Verificați tabloul de bord de sănătate a serviciului](https://portal.office.com/adminportal/home#/servicehealth).


