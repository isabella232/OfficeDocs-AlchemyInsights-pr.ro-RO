---
title: Limita zilnică de e-mail depășită. Fluxul de lucru este suspendat.
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
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731575"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="d7cc3-103">Limita zilnică de e-mail depășită.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="d7cc3-104">Fluxul de lucru este suspendat.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-104">Workflow is suspended.</span></span>

<span data-ttu-id="d7cc3-105">Această eroare poate fi primită în următoarele scenarii:</span><span class="sxs-lookup"><span data-stu-id="d7cc3-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="d7cc3-106">Aveți un flux de lucru în SharePoint Online care utilizează tipul de platformă de flux de lucru SharePoint 2010 sau SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="d7cc3-107">Fluxul de lucru este configurat pentru a trimite un mesaj de e-mail particularizat la mai mult de 200 de utilizatori la un moment dat, mai mult de 10.000 de destinatari pe zi sau mai mult de 30 de mesaje pe minut.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="d7cc3-108">Atunci când rulează fluxul de lucru, mesajul de e-mail nu este trimis și observați următorul comportament:</span><span class="sxs-lookup"><span data-stu-id="d7cc3-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="d7cc3-109">Pentru un flux de lucru utilizând tipul de platformă SharePoint 2013, navigați la pagina **stare flux de lucru** .</span><span class="sxs-lookup"><span data-stu-id="d7cc3-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="d7cc3-110">În pagina stare flux de lucru, **starea internă** este setată la **început**și balonul de informații **nu se afișează în imposibilitatea de a-l trimite unui destinatar**.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="d7cc3-111">Pentru a rezolva această problemă, configurați fluxul de lucru pentru a trimite mesaje de e-mail fără a depăși [limitele expeditorului Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="d7cc3-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="d7cc3-112">De exemplu, utilizați o pauză în fluxul de lucru, trimiteți e-mailul la un grup Microsoft 365, la un grup de distribuire sau la un grup de securitate cu e-mail activat sau trimiteți mesajul la mai puțin de 200 de destinatari odată.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="d7cc3-113">Pentru mai multe informații, consultați [articolul](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)următor.</span><span class="sxs-lookup"><span data-stu-id="d7cc3-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d7cc3-114">Subiecte asociate</span><span class="sxs-lookup"><span data-stu-id="d7cc3-114">Related topics</span></span>
- [<span data-ttu-id="d7cc3-115">Crearea fluxului</span><span class="sxs-lookup"><span data-stu-id="d7cc3-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d7cc3-116">SharePoint și fluxul</span><span class="sxs-lookup"><span data-stu-id="d7cc3-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 