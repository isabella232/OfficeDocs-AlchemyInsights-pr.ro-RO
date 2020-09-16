---
title: Adăugarea unui grup la un site SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771220"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleme la crearea unui site conectat la un grup în SharePoint

1. Au apărut câteva probleme comune atunci când creați sau creați din nou un site conectat la grup.
Dacă ați șters un grup și site-ul său conectat și doriți să creați un alt site cu același URL, va trebui să eliminați definitiv site-ul anterior.

   - Descărcați [componenta de administrare SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Pentru mai multe informații despre cum să începeți lucrul cu PowerShell, consultați [Introducere în componenta de administrare SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Eliminați site-ul din site-uri șterse utilizând cmdletul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell este necesar pentru a șterge definitiv site-urile de grup.

1. Dacă creați un site conectat la un grup și primiți un avertisment: **un alt grup cu același alias există deja**, bifați grupurile existente din centrul de [administrare Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Pentru a rezolva problema, ștergeți grupul existent dacă nu mai este necesar sau creați site-ul cu un alias diferit atribuit.

1. Există mai multe modalități de a crea și de a utiliza grupuri moderne cu SharePoint.

   - Puteți conecta site-urile existente la un grup Microsoft 365. Pentru mai multe informații, consultați [Conectarea unui grup Microsoft 365 utilizând interfața de utilizator SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Pentru a crea un site conectat la Microsoft 365 Group, va trebui să creați un [site de echipă](https://admin.microsoft.com/sharepoint).
