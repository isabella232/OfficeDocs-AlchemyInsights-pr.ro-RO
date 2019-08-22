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
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="108e2-102">Probleme atunci când crearea sau grup conectat sites înăuntru SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="108e2-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="108e2-103">Există o serie de probleme comune întâlnite atunci când crearea sau re-crearea unui grup de site-ul conectat.</span><span class="sxs-lookup"><span data-stu-id="108e2-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="108e2-104">Dacă aţi şters un grup şi site-ul său conectat şi doresc pentru a crea un alt site cu aceeaşi adresă URL, trebuie să eliminaţi definitiv site-ul anterior.</span><span class="sxs-lookup"><span data-stu-id="108e2-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="108e2-105">Descarca [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="108e2-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="108e2-106">Pentru mai multe informaţii despre Noţiuni de bază cu powershell, consultaţi [Noţiuni de SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="108e2-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="108e2-107">Eliminaţi situl urile şterse utilizând cmdlet-ul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.</span><span class="sxs-lookup"><span data-stu-id="108e2-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="108e2-108">Dacă creaţi un grup de site-ul conectat şi primiţi un avertisment există deja un alt grup cu acelaşi pseudonim, verifica grupuri existente din [Office 365 din centrul de administrare](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="108e2-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="108e2-109">Pentru a rezolva problema, ştergeţi grupul existent, în cazul în care mai este necesară sau pentru a crea site-ul cu un pseudonim diferite asociate.</span><span class="sxs-lookup"><span data-stu-id="108e2-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="108e2-110">Există diferite moduri de a crea şi de a folosi grupuri moderne cu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="108e2-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="108e2-111">Vă puteţi conecta site-urilor existente la un grup de Office 365.</span><span class="sxs-lookup"><span data-stu-id="108e2-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="108e2-112">Pentru mai multe informaţii, a se vedea [Conectarea unui grup de Office 365 utilizând SharePoint utilizator ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="108e2-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="108e2-113">Pentru a crea un site conectat de grup Office 365, trebuie să creaţi un Site de echipă.</span><span class="sxs-lookup"><span data-stu-id="108e2-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="108e2-114">Pentru mai multe informaţii, consultaţi [crearea unui site de echipă în SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="108e2-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

