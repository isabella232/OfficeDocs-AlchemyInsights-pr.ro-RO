---
title: înregistrarea apelurilor 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733861"
---
# <a name="11-call-recording"></a><span data-ttu-id="d1db5-102">înregistrarea apelurilor 1:1</span><span class="sxs-lookup"><span data-stu-id="d1db5-102">1:1 call recording</span></span>

<span data-ttu-id="d1db5-103">Administratorii trebuie să ia măsuri acum pentru a continua să le permiteți utilizatorilor să înregistreze apeluri 1:1.</span><span class="sxs-lookup"><span data-stu-id="d1db5-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="d1db5-104">Începând cu 12 aprilie, 2021, vom începe să impunem o opțiune nouă pentru Politica de apelare *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="d1db5-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="d1db5-105">În prezent, capacitățile de înregistrare a apelurilor 1:1 sunt controlate de opțiunea *AllowCloudRecording* în politicile pentru întâlnirile teams.</span><span class="sxs-lookup"><span data-stu-id="d1db5-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="d1db5-106">Dacă utilizatorilor li se permite să înregistreze întâlnirile teams, pot, de asemenea, înregistra apeluri 1:1.</span><span class="sxs-lookup"><span data-stu-id="d1db5-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="d1db5-107">Dacă preferați să blocați toți utilizatorii să înregistreze apeluri 1:1, nu trebuie să luați nicio acțiune.</span><span class="sxs-lookup"><span data-stu-id="d1db5-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="d1db5-108">Opțiunea politică de apelare *AllowCloudRecordingForCalls* va fi $false în mod implicit.</span><span class="sxs-lookup"><span data-stu-id="d1db5-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="d1db5-109">Această modificare este documentată în următoarea postare din centrul de mesaje: [(actualizat) 1:1 de înregistrare a politicii de înregistrare a apelurilor](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) pentru a seta opțiunea Team Calling Policy trebuie să utilizați [teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="d1db5-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="d1db5-110">**Pentru a activa înregistrarea apelurilor în 1:1 apeluri:** Set-CsTeamsCallingPolicy-Identity global-AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="d1db5-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="d1db5-111">**Pentru a dezactiva înregistrarea apelurilor în 1:1 apeluri:** Set-CsTeamsCallingPolicy-Identity global-AllowCloudRecordingForCalls $false</span><span class="sxs-lookup"><span data-stu-id="d1db5-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

