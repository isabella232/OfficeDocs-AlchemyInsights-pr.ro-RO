---
title: Adăugarea unui grup la un site SharePoint site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 396efbf9772b5398427a4fcc76e104fa95820af6
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532231"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Probleme comune la crearea unui site conectat la grup în SharePoint

1. Dacă ați șters un grup și site-ul conectat și doriți să creați alt site cu același URL, va trebui să eliminați definitiv site-ul anterior.

   - Descărcarea [shell-ului de administrare SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Pentru mai multe informații despre cum să începeți lucrul cu Powershell, consultați [Noțiuni de bază pentru SharePoint de administrare online.](/powershell/module/sharepoint-online/remove-sposite)
   - Eliminați site-ul din Site-uri șterse folosind cmdletul Powershell [Remove-SPODeletedSite.](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell este necesar pentru a șterge definitiv site-urile de grup.

1. Dacă creați un site conectat la grup și primiți un avertisment: Există deja un alt grup cu același **alias**, verificați grupurile existente din [Centru de administrare Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Pentru a rezolva problema, ștergeți grupul existent dacă nu mai este necesar sau creați site-ul cu un alt alias atribuit.

1. Există diverse modalități de a crea și a utiliza grupuri moderne cu SharePoint.

   - Puteți conecta site-uri existente la un Microsoft 365 grup. Pentru mai multe informații, [consultați Conectare a Microsoft 365 grup utilizând interfața utilizator SharePoint utilizator](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Pentru a crea Microsoft 365 site conectat la un grup de persoane, va trebui să creați un [Site de echipă.](https://admin.microsoft.com/sharepoint)
