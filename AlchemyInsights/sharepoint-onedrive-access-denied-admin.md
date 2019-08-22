---
title: Depanați mesajele de acces refuzat
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503548"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Depanarea Access Denied mesaje în centrul de administrare Sharepoint/OneDrive

Dacă vi se administrează un accent denied mesaj atunci când încearcă să navigaţi la un centru de administrare Sharepoint/OneDrive, vă rugăm să asiguraţi-vă că vă [atribuiţi o licenţă de utilizator](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). În cazul în care utilizatorul are o licenta, de asemenea, ar trebui să asiguraţi-vă că acestea se [atribuie un rol de administrator](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) care poate accesa centrele de admin.

Această problemă poate apărea când un utilizator este şters şi re-creat cu acelaşi nume principal de utilizator (UPN). Noul cont este creat folosind o valoare diferită de PUID (paşaport unic ID). Atunci când utilizatorul încearcă să acceseze o colecţie de site-ul sau lor OneDrive, utilizatorul are un PUID incorecte. Un al doilea scenariu implică sincronizare director cu o unitate organizaţională de Active Directory (OU). În cazul în care utilizatorii au deja conectat la SharePoint, apoi sa mutat la un OU diferite şi resynced cu SharePoint, acestea se pot confrunta aceasta problema.

Pentru a rezolva această problemă, trebuie să restabiliţi UPN original cu paşii din articol, [restaura un utilizator în Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Notă: În cazul în care un centru de OneDrive sau administrator SharePoint nu este disponibil pentru mai mulţi utilizatori care anterior a avut acces, poate fi o problemă temporară serviciu.  [Verificaţi tabloul de sănătate serviciu](https://portal.office.com/adminportal/home#/servicehealth).


