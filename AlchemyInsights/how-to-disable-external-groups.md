---
title: se dezactivează grupuri externe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720780"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="66069-102">se dezactivează grupuri externe</span><span class="sxs-lookup"><span data-stu-id="66069-102">How to disable External Groups</span></span>

<span data-ttu-id="66069-103">Yammer mesagerie externă aplică Reguli de transport Exchange (ETRs), un set de controale proactive pentru a preveni informațiile companiei de a fi partajate.</span><span class="sxs-lookup"><span data-stu-id="66069-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="66069-104">Pentru a restricționa utilizatorii să creeze grupuri externe, trebuie să configurați o regulă de transport Exchange (ETR), și apoi configurați Yammer pentru a utiliza regula Exchange Transport pentru a bloca mesageria externă.</span><span class="sxs-lookup"><span data-stu-id="66069-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="66069-105">După ce ați creat o regulă în centrul de administrare Exchange Online, urmați acești pași pentru a seta ETR să se aplice în Yammer:</span><span class="sxs-lookup"><span data-stu-id="66069-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="66069-106">Faceți Log on la Yammer ca administrator verificat, iar în **centrul de administrare Yammer**, accesați \*\*C Setări de securitate conținut și securitate. \> \*\*</span><span class="sxs-lookup"><span data-stu-id="66069-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="66069-107">Sub **Mesagerie externă**, **selectați Impuneți regulile de transport Exchange Online Exchange (ETRs) în Yammer.**</span><span class="sxs-lookup"><span data-stu-id="66069-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="66069-108">Alegeți **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="66069-108">Choose **Save**.</span></span>

<span data-ttu-id="66069-109">Pentru mai multe informații, consultați [Dezactivarea mesageriei externe într-o rețea Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="66069-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  