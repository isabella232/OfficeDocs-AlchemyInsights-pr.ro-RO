---
title: Începeţi cu SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770574"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="5104b-102">Fluxuri de lucru în SharePoint</span><span class="sxs-lookup"><span data-stu-id="5104b-102">Workflows in SharePoint</span></span>

<span data-ttu-id="5104b-103">În cazul în care fluxurile de lucru SharePoint nu trimit e-mailuri, organizaţia poate au întâmpinat limitele expeditorului Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="5104b-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="5104b-104">"Flux de lucru este suspendat" mesaj de eroare poate să apară dacă aveţi unul dintre următoarele elemente:</span><span class="sxs-lookup"><span data-stu-id="5104b-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="5104b-105">Ai un flux de lucru SharePoint Online care utilizează SharePoint 2010 sau tipul de platforma de flux de lucru SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="5104b-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="5104b-106">Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail personalizate pentru mai mult de 200 de utilizatori la un moment dat, peste 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.</span><span class="sxs-lookup"><span data-stu-id="5104b-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="5104b-107">Atunci când executaţi fluxul de lucru, nu este trimis mesajul de e-mail şi observaţi mesajul de eroare, starea internă este setată la suspendată sau imposibil de a trimite către un destinatar este afişat.</span><span class="sxs-lookup"><span data-stu-id="5104b-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="5104b-108">Pentru mai multe informaţii, consultaţi următorul [articol](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="5104b-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

