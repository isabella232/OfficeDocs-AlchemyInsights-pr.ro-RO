---
title: Depanarea mesajelor de acces refuzat
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051437"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Depanarea mesajelor de acces refuzat în SharePoint/OneDrive Admin Center

Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un centru de administrare SharePoint/OneDrive, asigurați-vă că [atribuiți o licență pentru utilizator](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Dacă utilizatorul are o licență, de asemenea, trebuie să vă asigurați că sunt [atribuite un rol de administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) care pot accesa centrele de administrare.

Această problemă poate apărea, de asemenea, atunci când un utilizator este șters și re-creat cu același nume principal de utilizator (UPN). Noul cont este creat utilizând un alt PUID (pașaport Unique ID) valoare. Când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive lor, utilizatorul are un PUID incorect. Un al doilea scenariu implică sincronizare director cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint și apoi sunt mutate într-un ou diferit și traducerea cu SharePoint, acestea pot experimenta această problemă.

Pentru a rezolva această problemă, ar trebui să restaurați UPN originală cu pașii din articol, [restaurați un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Notă: dacă un centru de administrare OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut anterior acces, poate exista o problemă de serviciu temporar.  [Verificați tabloul de bord de sănătate Service](https://portal.office.com/adminportal/home#/servicehealth).


