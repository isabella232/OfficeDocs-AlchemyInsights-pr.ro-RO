---
title: Depanarea mesajelor Access refuzate
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085240"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Depanarea accesului Mesajelor refuzate în Centrul de administrare SharePoint/OneDrive

Dacă primiți un mesaj de acces refuzat atunci când încercați să navigați la un Centru de administrare Sharepoint/OneDrive, asigurați-vă că îi atribuiți o [licență utilizatorului.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Dacă utilizatorul are o licență, trebuie, de asemenea, să vă asigurați că i se atribuie un [rol de administrator](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) care poate accesa centrele de administrare.

Această problemă poate apărea și atunci când un utilizator este șters și creat din nou cu același nume principal de utilizator (UPN). Noul cont este creat utilizând o altă valoare PUID (Pașaport unic). Atunci când utilizatorul încearcă să acceseze o colecție de site-uri sau OneDrive său, utilizatorul are un PUID incorect. Al doilea scenariu implică sincronizarea directorului cu o unitate organizațională Active Directory (OU). Dacă utilizatorii s-au conectat deja la SharePoint, apoi sunt mutati la un alt OU și sunt resincroniți cu SharePoint, aceștia pot experimenta această problemă.

Pentru a rezolva această problemă, trebuie să restaurați UPN-ul original cu pașii din articol Restaurarea [unui utilizator în Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Notă: Dacă un OneDrive un SharePoint nu este disponibil pentru mai mulți utilizatori care au avut acces anterior, poate exista o problemă temporară cu serviciul.  [Verificați tabloul de bord cu starea serviciilor](https://portal.office.com/adminportal/home#/servicehealth).


