---
title: Adăugaţi un grup la un sit SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507859"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Probleme atunci când crearea sau grup conectat sites înăuntru SharePoint Online

Există o serie de probleme comune întâlnite atunci când crearea sau re-crearea unui grup de site-ul conectat.

 Dacă aţi şters un grup şi site-ul său conectat şi doresc pentru a crea un alt site cu aceeaşi adresă URL, trebuie să eliminaţi definitiv site-ul anterior.

Descarca [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Pentru mai multe informaţii despre Noţiuni de bază cu powershell, consultaţi [Noţiuni de SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Eliminaţi situl urile şterse utilizând cmdlet-ul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.

Dacă creaţi un grup de site-ul conectat şi primiţi un avertisment există deja un alt grup cu acelaşi pseudonim, verifica grupuri existente din [Office 365 din centrul de administrare](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Pentru a rezolva problema, ştergeţi grupul existent, în cazul în care mai este necesară sau pentru a crea site-ul cu un pseudonim diferite asociate.

Există diferite moduri de a crea şi de a folosi grupuri moderne cu SharePoint.

Vă puteţi conecta site-urilor existente la un grup de Office 365. Pentru mai multe informaţii, a se vedea [Conectarea unui grup de Office 365 utilizând SharePoint utilizator ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Pentru a crea un site conectat de grup Office 365, trebuie să creaţi un Site de echipă. Pentru mai multe informaţii, consultaţi [crearea unui site de echipă în SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

