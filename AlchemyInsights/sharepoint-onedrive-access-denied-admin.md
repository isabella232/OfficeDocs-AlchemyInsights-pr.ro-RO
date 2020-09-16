---
title: Depanarea mesajelor interzise în Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767674"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Depanarea mesajelor refuzate în centrul de administrare SharePoint/OneDrive

Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un centru de administrare SharePoint/OneDrive, asigurați-vă că [atribuiți o licență pentru utilizator](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Dacă utilizatorul are o licență, trebuie, de asemenea, să vă asigurați că i se [atribuie un rol de administrator](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) care poate accesa centrele de administrare.

Această problemă poate apărea și atunci când un utilizator este șters și recreat cu același nume principal de utilizator (UPN). Noul cont este creat utilizând o altă valoare PUID (ID unic Passport). Atunci când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive, utilizatorul are o PUID incorectă. Un al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint, apoi sunt mutați la alt OU și Resincronizați cu SharePoint, este posibil ca aceștia să întâmpine această problemă.

Pentru a rezolva această problemă, trebuie să restaurați UPN-ul inițial cu pașii din articol, să [restaurați un utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Notă: dacă un centru de administrare OneDrive sau SharePoint nu este disponibil pentru mai mulți utilizatori care au avut acces anterior, este posibil să existe o problemă de serviciu temporară.  [Verificați tabloul de bord pentru starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).


