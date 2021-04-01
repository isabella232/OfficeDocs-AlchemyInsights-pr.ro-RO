---
title: Setați Microsoft Edge ca browser implicit pe un dispozitiv cu domeniu unit
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491881"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="083ff-102">Setați Microsoft Edge ca browser implicit pe un dispozitiv cu domeniu unit</span><span class="sxs-lookup"><span data-stu-id="083ff-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="083ff-103">Setați Microsoft Edge ca browser implicit:</span><span class="sxs-lookup"><span data-stu-id="083ff-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="083ff-104">[Creați un fișier de configurare cu asocieri implicite și](https://go.microsoft.com/fwlink/?linkid=2132437) stocați-l local sau într-o partajare de rețea.</span><span class="sxs-lookup"><span data-stu-id="083ff-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="083ff-105">Deschideți editorul de Politică de grup, apoi accesați **Computer Configuration**  >  **Administrative Templates** Windows  >  **Components** File  >  **Explorer**.</span><span class="sxs-lookup"><span data-stu-id="083ff-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="083ff-106">Selectați **Setați un fișier de configurare cu asocieri implicite.**</span><span class="sxs-lookup"><span data-stu-id="083ff-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="083ff-107">Selectați **Setare** politică , apoi **selectați Activat**.</span><span class="sxs-lookup"><span data-stu-id="083ff-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="083ff-108">Sub **Opțiuni,** introduceți locația fișierului de configurare cu asocieri implicite, apoi selectați **OK.**</span><span class="sxs-lookup"><span data-stu-id="083ff-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
