---
title: Blocat în Outbox din cauza atașamente mari
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441317"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="57e47-102">Remedierea mesajelor blocate în Outbox</span><span class="sxs-lookup"><span data-stu-id="57e47-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="57e47-103">Vă recomandăm să începeți prin rularea scenariului ["am probleme cu trimiterea, primirea sau găsirea mesajelor de e-mail"](https://aka.ms/SaRA-OutlookSendReceive) din instrumentul [Asistență Microsoft și asistent recuperare](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="57e47-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="57e47-104">Când un mesaj se blochează în Outbox, cele mai probabile cauze sunt:</span><span class="sxs-lookup"><span data-stu-id="57e47-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="57e47-105">Atașamente mari.</span><span class="sxs-lookup"><span data-stu-id="57e47-105">Large attachments.</span></span>
- <span data-ttu-id="57e47-106">Opțiunea **Trimitere imediată când este conectată** nu este activată.</span><span class="sxs-lookup"><span data-stu-id="57e47-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="57e47-107">Pentru a elimina atașamentele mari:</span><span class="sxs-lookup"><span data-stu-id="57e47-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="57e47-108">În Outlook, selectați **Trimitere/primire** > **lucru offline**.</span><span class="sxs-lookup"><span data-stu-id="57e47-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="57e47-109">În panoul de navigare, selectați **Outbox**.</span><span class="sxs-lookup"><span data-stu-id="57e47-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="57e47-110">De aici, puteți:</span><span class="sxs-lookup"><span data-stu-id="57e47-110">From here, you can:</span></span> 
    - <span data-ttu-id="57e47-111">Ștergeți mesajul (selectați-l și apoi selectați **Ștergere**).</span><span class="sxs-lookup"><span data-stu-id="57e47-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="57e47-112">Glisați mesajul în folderul Schițe, faceți dublu clic pentru a-l deschide și eliminați atașamentul, selectați-l și apoi selectați **Ștergere**).</span><span class="sxs-lookup"><span data-stu-id="57e47-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="57e47-113">Dacă primiți o eroare care spune că Outlook încearcă să transmită mesajul, închideți Outlook.</span><span class="sxs-lookup"><span data-stu-id="57e47-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="57e47-114">Este posibil să dureze câteva momente pentru a ieși.</span><span class="sxs-lookup"><span data-stu-id="57e47-114">It may take a few moments to exit.</span></span> <span data-ttu-id="57e47-115">Dacă Outlook nu se închide, apăsați Ctrl + Alt + Delete și selectați **Start Task Manager**.</span><span class="sxs-lookup"><span data-stu-id="57e47-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="57e47-116">În Task Manager, selectați fila **procese** , derulați în jos la Outlook. exe și selectați **Terminare proces**.</span><span class="sxs-lookup"><span data-stu-id="57e47-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="57e47-117">După ce Outlook se închide, reporniți-l și repetați pașii 2 și 3.</span><span class="sxs-lookup"><span data-stu-id="57e47-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="57e47-118">După ce eliminați atașarea, faceți clic pe **Trimitere/primire** > **lucru offline** pentru a relua lucrul online.</span><span class="sxs-lookup"><span data-stu-id="57e47-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="57e47-119">De asemenea, mesajele se blochează în Outbox când faceți clic pe **Trimitere**, dar nu sunteți conectat.</span><span class="sxs-lookup"><span data-stu-id="57e47-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="57e47-120">Apasă pe **trimite/primește** și uită-te la butonul de **lucru offline** .</span><span class="sxs-lookup"><span data-stu-id="57e47-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="57e47-121">Dacă e albastru, ești deconectat.</span><span class="sxs-lookup"><span data-stu-id="57e47-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="57e47-122">Selectați-l pentru a vă conecta (butonul devine alb) și faceți clic pe **Trimitere toate**.</span><span class="sxs-lookup"><span data-stu-id="57e47-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="57e47-123">Pentru a activa **trimiterea imediată când este conectată**:</span><span class="sxs-lookup"><span data-stu-id="57e47-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="57e47-124">Selectați \*\*\*\* > \*\*\*\* opțiunile >  de fișier**avansate**.</span><span class="sxs-lookup"><span data-stu-id="57e47-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="57e47-125">În secțiunea **Trimitere și primire** , selectați **Trimiteți imediat când sunteți conectat**, apoi alegeți **OK**.</span><span class="sxs-lookup"><span data-stu-id="57e47-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="57e47-126">Pentru detalii complete, a se vedea:</span><span class="sxs-lookup"><span data-stu-id="57e47-126">For full details see:</span></span>
- [<span data-ttu-id="57e47-127">Videoclip: trimiteți sau ștergeți un e-mail blocat</span><span class="sxs-lookup"><span data-stu-id="57e47-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="57e47-128">E-mail rămâne în folderul Outbox până când inițiați manual o operațiune de trimitere/primire în Outlook</span><span class="sxs-lookup"><span data-stu-id="57e47-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
