---
title: Introducere în SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766903"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="e19c5-102">Fluxuri de lucru în SharePoint</span><span class="sxs-lookup"><span data-stu-id="e19c5-102">Workflows in SharePoint</span></span>

<span data-ttu-id="e19c5-103">Dacă fluxurile de lucru SharePoint nu trimit e-mailuri, este posibil ca organizația să fi întâlnit limitele expeditorului Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e19c5-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="e19c5-104">Mesajul de eroare "flux de lucru este suspendat" poate apărea dacă aveți unul dintre următoarele elemente:</span><span class="sxs-lookup"><span data-stu-id="e19c5-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="e19c5-105">Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă SharePoint 2010 sau SharePoint 2013 flux de lucru.</span><span class="sxs-lookup"><span data-stu-id="e19c5-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="e19c5-106">Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail personalizat la mai mult de 200 utilizatori la un moment dat, mai mult de 10.000 destinatari pe zi, sau mai mult de 30 de mesaje pe minut.</span><span class="sxs-lookup"><span data-stu-id="e19c5-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="e19c5-107">Când executați fluxul de lucru, mesajul de poștă electronică nu este trimis și observați mesajul de eroare, starea internă este setată la suspendat sau imposibil de trimis la un destinatar este afișat.</span><span class="sxs-lookup"><span data-stu-id="e19c5-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="e19c5-108">Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="e19c5-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

