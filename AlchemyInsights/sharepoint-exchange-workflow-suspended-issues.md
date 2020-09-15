---
title: Introducere în SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700719"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="1f1ef-102">Fluxuri de lucru în SharePoint</span><span class="sxs-lookup"><span data-stu-id="1f1ef-102">Workflows in SharePoint</span></span>

<span data-ttu-id="1f1ef-103">Dacă fluxurile de lucru SharePoint nu trimit mesaje de e-mail, este posibil ca organizația să fi întâlnit limitele expeditorului Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1f1ef-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="1f1ef-104">Mesajul de eroare "fluxul de lucru este suspendat" poate apărea dacă aveți unul dintre următoarele elemente:</span><span class="sxs-lookup"><span data-stu-id="1f1ef-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="1f1ef-105">Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă de flux de lucru SharePoint 2010 sau SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="1f1ef-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="1f1ef-106">Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail particularizat la mai mult de 200 de utilizatori la un moment dat, mai mult de 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.</span><span class="sxs-lookup"><span data-stu-id="1f1ef-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="1f1ef-107">Atunci când rulează fluxul de lucru, mesajul de e-mail nu este trimis și observați mesajul de eroare, starea internă este setată la suspendat sau nu se poate trimite către un destinatar.</span><span class="sxs-lookup"><span data-stu-id="1f1ef-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="1f1ef-108">Pentru mai multe informații, vă rugăm să consultați următorul [articol](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="1f1ef-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

