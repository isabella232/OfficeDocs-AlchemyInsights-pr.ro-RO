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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314396"
---
# <a name="11-call-recording"></a>Înregistrarea apelurilor 1:1

Dacă butonul **Începere înregistrare** este estompat într-un apel 1:1, trebuie să modificați setările de politică pentru utilizatorul afectat. Pentru a verifica setarea politicii, rulați diagnostic pentru utilizatorul afectat **tastând Diag: Teams înregistrarea apelurilor 1:1 mai** sus.     

Începând cu 31 mai 2021, vom începe să impunem o nouă impunere a unei Teams de apelare internă *AllowCloudRecordingForCalls*. Înainte de această modificare, înregistrarea apelului 1:1 este controlată de *AllowCloudRecording* Teams Meeting Policy. Această modificare este documentată în postarea din Centrul de mesaje: [(Actualizat) 1:1 Introducere](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)în politica de înregistrare a apelurilor .  

*AllowCloudRecordingForCalls*   opțiunea politicii de apelare este setată la **$False** implicit. Dacă preferați să blocați înregistrarea apelurilor 1:1 de către toți utilizatorii, nu trebuie să luați nicio măsură.  

Pentru a activa înregistrarea apelurilor pentru toți utilizatorii în apeluri 1:1, [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) pentru a rula următorul cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Alternativ, puteți să creați o politică nouă și să setați **-AllowCloudRecordingForCalls** **la $true** și să atribuiți politica utilizatorilor dvs. 

Pentru mai multe informații, consultați [1:1 Controalele politicii de înregistrare a apelurilor sunt (aproape!) Aici](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
