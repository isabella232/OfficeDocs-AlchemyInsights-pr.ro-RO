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
# <a name="11-call-recording"></a>înregistrarea apelurilor 1:1

Administratorii trebuie să ia măsuri acum pentru a continua să le permiteți utilizatorilor să înregistreze apeluri 1:1.
 
Începând cu 12 aprilie, 2021, vom începe să impunem o opțiune nouă pentru Politica de apelare *AllowCloudRecordingForCalls*. 

În prezent, capacitățile de înregistrare a apelurilor 1:1 sunt controlate de opțiunea *AllowCloudRecording* în politicile pentru întâlnirile teams. Dacă utilizatorilor li se permite să înregistreze întâlnirile teams, pot, de asemenea, înregistra apeluri 1:1.

Dacă preferați să blocați toți utilizatorii să înregistreze apeluri 1:1, nu trebuie să luați nicio acțiune. Opțiunea politică de apelare *AllowCloudRecordingForCalls* va fi $false în mod implicit.

Această modificare este documentată în următoarea postare din centrul de mesaje: [(actualizat) 1:1 de înregistrare a politicii de înregistrare a apelurilor](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) pentru a seta opțiunea Team Calling Policy trebuie să utilizați [teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Pentru a activa înregistrarea apelurilor în 1:1 apeluri:** Set-CsTeamsCallingPolicy-Identity global-AllowCloudRecordingForCalls $True

**Pentru a dezactiva înregistrarea apelurilor în 1:1 apeluri:** Set-CsTeamsCallingPolicy-Identity global-AllowCloudRecordingForCalls $false

