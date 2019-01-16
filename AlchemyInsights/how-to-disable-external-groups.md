---
title: Cum se dezactivează grupurile externe
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306786"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="3c5f7-102">Cum se dezactivează grupurile externe</span><span class="sxs-lookup"><span data-stu-id="3c5f7-102">How to disable External Groups</span></span>

<span data-ttu-id="3c5f7-p101">Yammer mesagerie extern se aplică regulile de Transport Exchange (ETRs), un set de controale proactive pentru a preveni informaţii companie să fie partajate. Pentru a redenumi la crearea grupurilor de externe, trebuie să configuraţi o regulă de transport Exchange (ETR), şi apoi configuraţi Yammer pentru a utiliza regula de Exchange Transport pentru a bloca mesaje externe.</span><span class="sxs-lookup"><span data-stu-id="3c5f7-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="3c5f7-105">Odată ce aţi creat o regulă în centrul de administrare Exchange Online, urmaţi aceşti paşi pentru a seta ETR să se aplice în Yammer:</span><span class="sxs-lookup"><span data-stu-id="3c5f7-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="3c5f7-106">Conectaţi-vă la Yammer ca un admin verificate şi în **Centrul de administrare Yammer**, du-te la C **ontent şi securitate \> setările de securitate.**</span><span class="sxs-lookup"><span data-stu-id="3c5f7-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="3c5f7-107">**Externe de mesaje**, selectaţi **impune Transport Exchange Online schimb regulile (ETRs) în Yammer.**</span><span class="sxs-lookup"><span data-stu-id="3c5f7-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="3c5f7-108">Selectaţi **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="3c5f7-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="3c5f7-109">Pentru informaţii suplimentare, consultaţi [controlul extern mesaje într-o reţea de Yammer cu regulile de Exchange Transport](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="3c5f7-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

