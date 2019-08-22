---
title: Zi cu zi e-mail depăşit limita. Flux de lucru este suspendat.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514479"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="41e81-103">E-mail zilnic a depăşit limita.</span><span class="sxs-lookup"><span data-stu-id="41e81-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="41e81-104">Flux de lucru este suspendat.</span><span class="sxs-lookup"><span data-stu-id="41e81-104">Workflow is suspended.</span></span>

<span data-ttu-id="41e81-105">Această eroare poate fi primit în următoarele situaţii:</span><span class="sxs-lookup"><span data-stu-id="41e81-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="41e81-106">Ai un flux de lucru SharePoint Online care utilizează SharePoint 2010 sau tipul de platforma de flux de lucru SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="41e81-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="41e81-107">Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail personalizate pentru mai mult de 200 de utilizatori la un moment dat, peste 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.</span><span class="sxs-lookup"><span data-stu-id="41e81-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="41e81-108">Când executaţi fluxul de lucru, nu este trimis mesajul e-mail, şi observaţi următorul comportament:</span><span class="sxs-lookup"><span data-stu-id="41e81-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="41e81-109">Pentru un flux de lucru utilizând tipul de platforma SharePoint 2013, navigați la pagina **Stare flux de lucru** .</span><span class="sxs-lookup"><span data-stu-id="41e81-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="41e81-110">Pe pagina stare flux de lucru, **Starea internă** este setată la **începute**şi balonul cu informaţii afişează **nu se poate trimite la un destinatar**.</span><span class="sxs-lookup"><span data-stu-id="41e81-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="41e81-111">Pentru a rezolva această problemă, configuraţi fluxul de lucru pentru a trimite mesaje e-mail, fără a depăşi [limitele de expeditor Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="41e81-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="41e81-112">De exemplu, utilizaţi o pauză în fluxul de lucru, trimiteţi un email la un grup de Office 365, un grup de distribuire sau un grup de securitate mail activat sau trimite mesajul la mai puţin de 200 de destinatari la un moment dat.</span><span class="sxs-lookup"><span data-stu-id="41e81-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="41e81-113">Pentru informaţii suplimentare, consultaţi următorul [articol](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="41e81-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="41e81-114">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="41e81-114">Related topics</span></span>
- [<span data-ttu-id="41e81-115">Crea fluxul</span><span class="sxs-lookup"><span data-stu-id="41e81-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="41e81-116">SharePoint şi fluxul</span><span class="sxs-lookup"><span data-stu-id="41e81-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 