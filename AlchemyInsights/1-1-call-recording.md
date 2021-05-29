---
title: Înregistrarea apelurilor 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702102"
---
# <a name="11-call-recording"></a><span data-ttu-id="14042-102">Înregistrarea apelurilor 1:1</span><span class="sxs-lookup"><span data-stu-id="14042-102">1:1 call recording</span></span>

<span data-ttu-id="14042-103">Dacă butonul **Începere înregistrare** este estompat într-un apel 1:1, trebuie să modificați setările de politică pentru utilizatorul afectat.</span><span class="sxs-lookup"><span data-stu-id="14042-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="14042-104">Pentru a verifica setarea politicii, rulați diagnostic pentru utilizatorul afectat **tastând Diag: Teams înregistrarea apelurilor 1:1 mai** sus.</span><span class="sxs-lookup"><span data-stu-id="14042-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="14042-105">Începând cu 31 mai 2021, vom începe să impunem o nouă impunere a unei Teams de apelare internă *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="14042-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="14042-106">Înainte de această modificare, înregistrarea apelului 1:1 este controlată de *AllowCloudRecording* Teams Meeting Policy.</span><span class="sxs-lookup"><span data-stu-id="14042-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="14042-107">Această modificare este documentată în postarea din Centrul de mesaje: [(Actualizat) 1:1 Introducere](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)în politica de înregistrare a apelurilor .</span><span class="sxs-lookup"><span data-stu-id="14042-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="14042-108">*AllowCloudRecordingForCalls*   opțiunea politicii de apelare este setată la **$False** implicit.</span><span class="sxs-lookup"><span data-stu-id="14042-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="14042-109">Dacă preferați să blocați înregistrarea apelurilor 1:1 de către toți utilizatorii, nu trebuie să luați nicio măsură.</span><span class="sxs-lookup"><span data-stu-id="14042-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="14042-110">Pentru a activa înregistrarea apelurilor pentru toți utilizatorii în apeluri 1:1, [Teams PowerShell](/microsoftteams/teams-powershell-install) pentru a rula următorul cmdlet:</span><span class="sxs-lookup"><span data-stu-id="14042-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="14042-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="14042-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="14042-112">Alternativ, puteți să creați o politică nouă și să setați **-AllowCloudRecordingForCalls** **la $true** și să atribuiți politica utilizatorilor dvs.</span><span class="sxs-lookup"><span data-stu-id="14042-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="14042-113">Pentru mai multe informații, consultați [1:1 Controalele politicii de înregistrare a apelurilor sunt (aproape!) Aici](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="14042-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
