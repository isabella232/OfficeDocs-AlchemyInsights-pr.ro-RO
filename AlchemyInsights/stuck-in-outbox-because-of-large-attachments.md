---
title: Blocat în Outbox din cauza atașărilor mari
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241264"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="4d3bb-102">Remedierea mesajelor blocate în Outbox</span><span class="sxs-lookup"><span data-stu-id="4d3bb-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="4d3bb-103">Vă recomandăm să începeți prin a executa scenariul ["Am probleme cu trimiterea, primirea sau găsirea mesajelor de poștă electronică"](https://aka.ms/SaRA-OutlookSendReceive) din instrumentul [Asistent de asistență și recuperare Microsoft.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="4d3bb-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="4d3bb-104">Atunci când un mesaj devine blocat în Outbox, cauza cea mai probabilă este o atașare mare sau opțiunea "Trimite imediat atunci când este conectat" nu este activată.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="4d3bb-105">**Eliminarea atașării mari**</span><span class="sxs-lookup"><span data-stu-id="4d3bb-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="4d3bb-106">În Outlook, selectați **Trimitere / primire** > **de lucru offline**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="4d3bb-107">În panoul de navigare, selectați **Outbox**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="4d3bb-108">De aici, puteți:</span><span class="sxs-lookup"><span data-stu-id="4d3bb-108">From here, you can:</span></span> 
    - <span data-ttu-id="4d3bb-109">ºtergeþi mesajul (selectaþi-l ºi apoi **selectaþi ªtergeþi**).</span><span class="sxs-lookup"><span data-stu-id="4d3bb-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="4d3bb-110">Glisați mesajul în folderul Schițe, faceți dublu clic pentru a-l deschide și eliminați atașarea, selectați-l, apoi **selectați Ștergere**).</span><span class="sxs-lookup"><span data-stu-id="4d3bb-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="4d3bb-111">Dacă primiți o eroare care spune Outlook încearcă să transmită mesajul, închideți Outlook.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="4d3bb-112">S-ar putea să dureze câteva momente să iasă.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-112">It may take a few moments to exit.</span></span> <span data-ttu-id="4d3bb-113">Dacă Outlook nu se închide, apăsați Ctrl+Alt+Delete și selectați **Pornire Manager activități**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="4d3bb-114">În Managerul de activități, selectați fila **Procese,** defilați în jos la outlook.exe și selectați **Terminare proces**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="4d3bb-115">După ce Outlook se închide, reporniți-l și repetați pașii 2 și 3.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="4d3bb-116">După ce eliminați atașarea, faceți clic pe **Trimitere / primire** > **lucru offline** pentru a relua lucrul online.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="4d3bb-117">Mesajele rămân blocate și în Outbox când faceți clic pe **Trimitere**, dar nu sunteți conectat.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="4d3bb-118">Faceți clic pe **Trimitere / Primire** și uitați-vă la butonul Lucru **offline.**</span><span class="sxs-lookup"><span data-stu-id="4d3bb-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="4d3bb-119">Dacă e albastru, ești deconectat.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="4d3bb-120">Faceți clic pe ea pentru a vă conecta (butonul devine alb) și faceți clic pe **Trimitere totală**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="4d3bb-121">**Activare trimitere imediat după conectare**</span><span class="sxs-lookup"><span data-stu-id="4d3bb-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="4d3bb-122">Pe fila Fișier, faceți clic pe **Opțiuni**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="4d3bb-123">În caseta de dialog Opțiuni Outlook, faceți clic pe **Complex**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="4d3bb-124">În secțiunea Trimitere și primire, faceți clic pentru a activa **Trimitere imediat când este conectat**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="4d3bb-125">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="4d3bb-125">Click **OK**.</span></span>
 
<span data-ttu-id="4d3bb-126">Pentru detalii complete, consultați:</span><span class="sxs-lookup"><span data-stu-id="4d3bb-126">For full details, see:</span></span>
- [<span data-ttu-id="4d3bb-127">Video: Trimiterea sau ștergerea unui e-mail blocat</span><span class="sxs-lookup"><span data-stu-id="4d3bb-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="4d3bb-128">E-mailrămâne în folderul Outbox până când inițiați manual o operațiune de trimitere / primire în Outlook</span><span class="sxs-lookup"><span data-stu-id="4d3bb-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
