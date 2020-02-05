---
title: Adăugarea unui grup la un site SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770363"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleme la crearea unui site conectat la grup în SharePoint

1. Unele probleme comune întâlnite la crearea sau recrearea unui site conectat la grup.
Dacă ați șters un grup și site-ul său conectat și doriți să creați un alt site cu același URL, va trebui să eliminați definitiv site-ul anterior.

   - Descarca [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Pentru mai multe informații despre introducere în Powershell, consultați [Introducere în Componenta de gestionare SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Eliminați site-ul din site-uri șterse utilizând cmdletul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell . Powershell este necesar pentru a șterge definitiv site-uri de grup.

1. Dacă creați un site conectat la grup și primiți un avertisment: există deja un **alt grup cu același alias**, verificați grupurile existente din Office [365 din Centrul de administrare](https://admin.microsoft.com/AdminPortal/Home#/groups). Pentru a rezolva problema, ștergeți grupul existent dacă nu mai este necesar sau creați site-ul cu un alias diferit atribuit.

1. Există diferite moduri de a crea și de a utiliza grupuri moderne cu SharePoint.

   - Aveți posibilitatea să conectați site-uri existente la un grup Office 365. Pentru mai multe informații, consultați [Conectarea unui grup Office 365 utilizând interfața cu utilizatorul SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Pentru a crea un site conectat la grupul Office 365, va trebui să creați un site de [echipă](https://admin.microsoft.com/sharepoint).
