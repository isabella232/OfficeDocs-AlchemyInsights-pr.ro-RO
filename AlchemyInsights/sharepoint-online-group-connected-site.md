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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642156"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="f8e7e-102">Probleme la crearea unui grup conectat site-ul în SharePoint</span><span class="sxs-lookup"><span data-stu-id="f8e7e-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="f8e7e-103">Unele probleme comune întâlnite la crearea sau recrearea unui site conectat la grup.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="f8e7e-104">Dacă ați șters un grup și site-ul său conectat și doriți să creați un alt site cu același URL, va trebui să eliminați definitiv site-ul anterior.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="f8e7e-105">Descarca [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f8e7e-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="f8e7e-106">Pentru mai multe informații despre introducere în Powershell, consultați [Introducere în Componenta de administrare SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="f8e7e-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="f8e7e-107">Eliminați site-ul din site-uri șterse utilizând cmdletul [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="f8e7e-108">Powershell este necesar pentru a șterge definitiv site-urile de grup.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="f8e7e-109">Dacă creați un site conectat la grup și primiți un avertisment: **Există deja un alt grup cu același alias**, verificați grupurile existente din Centrul de administrare Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="f8e7e-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="f8e7e-110">Pentru a rezolva problema, ștergeți grupul existent dacă nu mai este necesar sau creați site-ul cu un alias diferit atribuit.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="f8e7e-111">Există diferite modalități de a crea și utiliza grupuri moderne cu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="f8e7e-112">Puteți conecta site-urile existente la un grup Office 365.</span><span class="sxs-lookup"><span data-stu-id="f8e7e-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="f8e7e-113">Pentru mai multe informații, consultați [Conectarea unui grup Office 365 utilizând interfața cu utilizatorul SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f8e7e-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="f8e7e-114">Pentru a crea un site conectat la grupul Office 365, va trebui să creați un [site de echipă](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f8e7e-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
