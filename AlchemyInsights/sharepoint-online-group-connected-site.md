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
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758742"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Crearea site-urilor conectate grup SharePoint Online

Există o serie de probleme comune întâlnite atunci când crearea sau re-crearea unui grup de site-ul conectat.

 Dacă aţi şters un grup şi site-ul său conectat şi doresc pentru a crea un alt site cu aceeaşi adresă URL, trebuie să eliminaţi definitiv site-ul anterior.

Descarca [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Pentru mai multe informaţii despre Noţiuni de bază cu powershell, consultaţi [Noţiuni de SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Eliminaţi situl urile şterse utilizând cmdlet-ul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.

Dacă creaţi un grup de site-ul conectat şi primiţi un avertisment există deja un alt grup cu acelaşi pseudonim, verifica grupuri existente din [Office 365 din centrul de administrare](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Pentru a rezolva problema, ştergeţi grupul existent, în cazul în care mai este necesară sau pentru a crea site-ul cu un pseudonim diferite asociate.

Există diferite moduri de a crea şi de a folosi grupuri moderne cu SharePoint.

Vă puteţi conecta site-urilor existente la un grup de Office 365. Pentru mai multe informaţii, a se vedea [Conectarea unui grup de Office 365 utilizând SharePoint utilizator ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Pentru a crea un site conectat de grup Office 365, trebuie să creaţi un Site de echipă. Pentru mai multe informaţii, consultaţi [crearea unui site de echipă în SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

