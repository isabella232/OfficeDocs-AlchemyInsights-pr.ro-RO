---
title: Adăugarea unui grup la un sit SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750532"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Probleme la crearea sau gruparea site-uri conectate în SharePoint Online

Există câteva probleme comune întâlnite la crearea sau recrearea unui site conectat la grup.

 Dacă ați șters un grup și site-ul său conectat și doriți să creați un alt site cu același URL, va trebui să eliminați definitiv site-ul anterior.

Descarca [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Pentru mai multe informații despre Noțiuni introductive despre PowerShell, consultați [Noțiuni introductive despre SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Eliminați site-ul din site-uri șterse utilizând cmdletul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.

Dacă creați un site conectat la grup și primiți un avertisment un alt grup cu același alias există deja, Verificați grupurile existente din [Office 365 de la centrul de administrare](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Pentru a rezolva problema, ștergeți grupul existent dacă nu mai este necesar sau creați site-ul cu un alias diferit atribuit.

Există diferite modalități de a crea și de a utiliza grupuri moderne cu SharePoint.

Aveți posibilitatea să conectați site-uri existente la un grup de Office 365. Pentru mai multe informații, consultați [Conectarea unui grup Office 365 utilizând utilizatorul SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Pentru a crea un site conectat la grupul Office 365, va trebui să creați un site de echipă. Pentru mai multe informații, consultați [crearea unui site de echipă în SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

