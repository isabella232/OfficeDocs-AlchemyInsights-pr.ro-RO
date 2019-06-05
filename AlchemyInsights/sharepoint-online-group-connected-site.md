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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719493"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Crearea site-urilor conectate grup SharePoint Online

<p><strong>Există o serie de probleme comune întâlnite atunci când crearea sau re-crearea unui grup de site-ul conectat.&nbsp;</strong></p>  <p>1.Dacă aţi şters un grup şi site-ul său conectat şi doresc pentru a crea un alt site cu aceeaşi adresă URL, trebuie să eliminaţi definitiv site-ul anterior.</p>  <ul>  <li>Descarca <a title="coajă de Management SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - pentru mai multe informaţii despre Noţiuni de bază cu powershell, consultaţi <a title="Noţiuni de bază cu SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Noţiuni de bază cu SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Elimina site-ul de la site-uri şterse folosind <a title="Remove-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remove-SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Dacă creaţi un grup de site-ul conectat şi primiţi un avertisment <strong>'există un alt grup cu acelaşi pseudonim deja'</strong>, verifica grupuri existente la <a title="Office 365 din centrul de administrare" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 din centrul de administrare</a>. Pentru a rezolva problema, ştergeţi grupul existent, în cazul în care mai este necesară sau pentru a crea site-ul cu un pseudonim diferite asociate.&nbsp;</p>  <p><strong>Există diferite moduri de a crea şi de a folosi grupuri moderne cu SharePoint.&nbsp;</strong></p>  <ol>  <li>Vă puteţi conecta site-urilor existente la un grup de Office 365. Pentru mai multe informaţii, consultaţi <a title="conecta un grup de Office 365 utilizând SharePoint utilizator ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Conectaţi un grup de Office 365 utilizând SharePoint utilizator ineterface</a>.</li>  <li>Pentru a crea un site conectat de grup Office 365, trebuie să creaţi un Site de echipă. Pentru mai multe informaţii, consultaţi <a title="a crea un site de echipă în SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Creați un site de echipă în SharePoint.</a></li>  </ol>

