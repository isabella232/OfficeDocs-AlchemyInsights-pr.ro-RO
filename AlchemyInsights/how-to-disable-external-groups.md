---
title: se dezactivează grupurile externe
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739505"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="eb345-102">se dezactivează grupurile externe</span><span class="sxs-lookup"><span data-stu-id="eb345-102">How to disable External Groups</span></span>

<span data-ttu-id="eb345-103">Mesageria externă Yammer aplică regulile de transport Exchange (ETRs), un set de controale proactive pentru a împiedica partajarea informațiilor companiei.</span><span class="sxs-lookup"><span data-stu-id="eb345-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="eb345-104">Pentru a restrânge utilizatorii să creeze grupuri externe, trebuie să configurați o regulă de transport Exchange (ETR), și apoi Configurați Yammer pentru a utiliza regula de schimb de transport pentru a bloca mesageria externă.</span><span class="sxs-lookup"><span data-stu-id="eb345-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="eb345-105">După ce ați creat o regulă în centrul de administrare Exchange Online, urmați acești pași pentru a seta ETR să se aplice în Yammer:</span><span class="sxs-lookup"><span data-stu-id="eb345-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="eb345-106">Faceți Log on la Yammer ca administrator verificat și în centrul de **administrare Yammer**, mergeți la C \*\*conținut și \> \*\* securitate de securitate setări.</span><span class="sxs-lookup"><span data-stu-id="eb345-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="eb345-107">Sub **Mesagerie externă**, selectați **aplicarea regulilor Exchange Online Exchange Transport (ETRs) în Yammer.**</span><span class="sxs-lookup"><span data-stu-id="eb345-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="eb345-108">Alegeți **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="eb345-108">Choose **Save**.</span></span>

<span data-ttu-id="eb345-109">Pentru mai multe informații, consultați [dezactivarea mesageriei externe într-o rețea Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="eb345-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  