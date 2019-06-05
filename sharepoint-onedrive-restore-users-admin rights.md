---
title: Accesul utilizatorilor la SharePoint și OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715223"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Accesul utilizatorilor la SharePoint și OneDrive

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Această problemă apare cel mai frecvent atunci când un utilizator este şters şi re-creat cu acelaşi nume principal de utilizator (UPN). Noul cont este creat folosind o valoare diferită de PUID (paşaport unic ID). Atunci când utilizatorul încearcă să acceseze o colecţie de site-ul sau lor OneDrive, utilizatorul are un PUID incorecte. Un al doilea scenariu implică sincronizare director cu o unitate organizaţională de Active Directory (OU). În cazul în care utilizatorii au deja conectat la SharePoint, apoi sa mutat la un OU diferite şi resynced cu SharePoint, acestea se pot confrunta aceasta problema.</span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Pentru a rezolva această problemă ar trebui să restabiliţi UPN original cu paşii din articol, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">restaura un utilizator în Office 365.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">După ce acest lucru este făcut, puteţi verifica dacă utilizatorul are drepturi de administrator la site-ul OneDrive urmând paşii de la <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Adauga admin pe pentru un utilizator OneDrive.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Pentru mai multe informaţii despre nivelurile de permisiune, a se vedea articolul, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">nivelurile de permisiune în SharePoint.</a>&nbsp;</span></p>
