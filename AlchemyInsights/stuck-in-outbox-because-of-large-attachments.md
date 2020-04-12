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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232642"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b444b-102">Remedierea mesajelor blocate în Outbox</span><span class="sxs-lookup"><span data-stu-id="b444b-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b444b-103">Vă recomandăm să începeți prin a executa scenariul ["Am probleme cu trimiterea, primirea sau găsirea mesajelor de poștă electronică"](https://aka.ms/SaRA-OutlookSendReceive) din instrumentul [Asistent de asistență și recuperare Microsoft](https://diagnostics.office.com/#/) de pe computerul afectat.</span><span class="sxs-lookup"><span data-stu-id="b444b-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="b444b-104">Atunci când un mesaj devine blocat în Outbox, cauza cea mai probabilă este o atașare mare sau opțiunea "Trimite imediat atunci când este conectat" nu este activată.</span><span class="sxs-lookup"><span data-stu-id="b444b-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="b444b-105">**Eliminarea atașării mari**</span><span class="sxs-lookup"><span data-stu-id="b444b-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="b444b-106">Faceți clic pe **Trimitere/ Primire** > **lucru offline**.</span><span class="sxs-lookup"><span data-stu-id="b444b-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b444b-107">În panoul de navigare, faceți clic pe **Outbox**.</span><span class="sxs-lookup"><span data-stu-id="b444b-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="b444b-108">De aici, puteți:</span><span class="sxs-lookup"><span data-stu-id="b444b-108">From here, you can:</span></span> 
    - <span data-ttu-id="b444b-109">Ștergeți mesajul.</span><span class="sxs-lookup"><span data-stu-id="b444b-109">Delete the message.</span></span> <span data-ttu-id="b444b-110">Trebuie doar să-l selectați și faceți clic pe **Ștergere**.</span><span class="sxs-lookup"><span data-stu-id="b444b-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="b444b-111">Glisați mesajul în **folderul schițe ,** faceți dublu clic pentru a deschide mesajul și ștergeți atașarea (faceți clic pe el și faceți clic pe **Ștergere**).</span><span class="sxs-lookup"><span data-stu-id="b444b-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="b444b-112">Dacă o eroare vă spune că Outlook încearcă să transmită mesajul, închideți Outlook.</span><span class="sxs-lookup"><span data-stu-id="b444b-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b444b-113">S-ar putea să dureze câteva momente să iasă.</span><span class="sxs-lookup"><span data-stu-id="b444b-113">It may take a few moments to exit.</span></span> <span data-ttu-id="b444b-114">Dacă Outlook nu se închide, **apăsați Ctrl+Alt+Delete** și faceți clic pe **Pornire Manager de activități**.</span><span class="sxs-lookup"><span data-stu-id="b444b-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="b444b-115">În Managerul de activități, selectați fila **Procese,** defilați în jos la outlook.exe și faceți clic pe **Terminare proces**.</span><span class="sxs-lookup"><span data-stu-id="b444b-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="b444b-116">După ce Outlook se închide, reporniți Outlook și repetați pașii 2-3.</span><span class="sxs-lookup"><span data-stu-id="b444b-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="b444b-117">După ce eliminați atașarea, faceți clic pe **Trimitere / primire** > **de lucru offline** pentru a deselecta butonul și pentru a relua lucrul online.</span><span class="sxs-lookup"><span data-stu-id="b444b-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="b444b-118">Mesajele rămân blocate și în Outbox când faceți clic pe **Trimitere**, dar nu sunteți conectat.</span><span class="sxs-lookup"><span data-stu-id="b444b-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b444b-119">Faceți clic pe **Trimitere / Primire** și uitați-vă la butonul Lucru **offline.**</span><span class="sxs-lookup"><span data-stu-id="b444b-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b444b-120">Dacă e albastru, ești deconectat.</span><span class="sxs-lookup"><span data-stu-id="b444b-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b444b-121">Faceți clic pe ea pentru a vă conecta (butonul devine alb) și faceți clic pe **Trimitere totală**.</span><span class="sxs-lookup"><span data-stu-id="b444b-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b444b-122">**Activare trimitere imediat după conectare**</span><span class="sxs-lookup"><span data-stu-id="b444b-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="b444b-123">Pe fila Fișier, faceți clic pe **Opțiuni**.</span><span class="sxs-lookup"><span data-stu-id="b444b-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="b444b-124">În caseta de dialog Opțiuni Outlook, faceți clic pe **Complex**.</span><span class="sxs-lookup"><span data-stu-id="b444b-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="b444b-125">În secțiunea Trimitere și primire, faceți clic pentru a activa **Trimitere imediat când este conectat**.</span><span class="sxs-lookup"><span data-stu-id="b444b-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="b444b-126">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="b444b-126">Click **OK**.</span></span>
 
<span data-ttu-id="b444b-127">Pentru detalii complete, consultați:</span><span class="sxs-lookup"><span data-stu-id="b444b-127">For full details, see:</span></span>
- [<span data-ttu-id="b444b-128">Video: Trimiterea sau ștergerea unui e-mail blocat</span><span class="sxs-lookup"><span data-stu-id="b444b-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b444b-129">E-mailrămâne în folderul Outbox până când inițiați manual o operațiune de trimitere / primire în Outlook</span><span class="sxs-lookup"><span data-stu-id="b444b-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
