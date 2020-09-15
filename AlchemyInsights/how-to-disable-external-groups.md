---
title: Cum se dezactivează grupurile externe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704140"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="6f348-102">Cum se dezactivează grupurile externe</span><span class="sxs-lookup"><span data-stu-id="6f348-102">How to disable External Groups</span></span>

<span data-ttu-id="6f348-103">Mesageria externă Yammer aplică regulile de transport Exchange (ETRs), un set de controale proactiv pentru a împiedica partajarea informațiilor firmei.</span><span class="sxs-lookup"><span data-stu-id="6f348-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="6f348-104">Pentru a restricționa utilizatorii să creeze grupuri externe, trebuie să configurați o regulă de transport Exchange (ETR), apoi să configurați Yammer pentru a utiliza regula de transport Exchange pentru a bloca mesageria externă.</span><span class="sxs-lookup"><span data-stu-id="6f348-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="6f348-105">După ce ați creat o regulă în centrul de administrare Exchange Online, urmați acești pași pentru a seta ETR să se aplice în Yammer:</span><span class="sxs-lookup"><span data-stu-id="6f348-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="6f348-106">Conectați-vă la Yammer ca administrator verificat și, în **Centrul de administrare Yammer**, accesați setările C pentru \*\*conținut și \> \*\* securitate de securitate.</span><span class="sxs-lookup"><span data-stu-id="6f348-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="6f348-107">Sub **Mesagerie externă**, selectați **aplicați regulile de transport Exchange Online Exchange (ETRs) în Yammer.**</span><span class="sxs-lookup"><span data-stu-id="6f348-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="6f348-108">Alegeți **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="6f348-108">Choose **Save**.</span></span>

<span data-ttu-id="6f348-109">Pentru mai multe informații, consultați [dezactivarea mesageriei externe într-o rețea Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="6f348-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  