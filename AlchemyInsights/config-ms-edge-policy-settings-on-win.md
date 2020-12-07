---
title: Configurarea setărilor politicii Microsoft Edge în Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583742"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="c263f-102">Configurarea setărilor politicii Microsoft Edge în Windows</span><span class="sxs-lookup"><span data-stu-id="c263f-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="c263f-103">Pentru a configura setările de politică și actualizările gestionate pentru Microsoft Edge, utilizați obiecte politică de grup (GPO).</span><span class="sxs-lookup"><span data-stu-id="c263f-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="c263f-104">De asemenea, puteți să furnizați politici prin registry; Acest lucru ar fi potrivit pentru (1) dispozitivele Windows s-au alăturat unui domeniu Microsoft Active Directory și pentru (2) instanțele Windows 10 Pro și Enterprise înscrise pentru gestionarea dispozitivelor în Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c263f-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="c263f-105">Pentru a configura Microsoft Edge utilizând GPO, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="c263f-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="c263f-106">La magazinul central al politicii de grup din domeniul Active Directory sau la folderul șablon de definiție politică de pe computere individuale, instalați toate șabloanele administrative care adaugă reguli și setări pentru Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="c263f-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="c263f-107">Configurați politicile specifice pe care doriți să le setați.</span><span class="sxs-lookup"><span data-stu-id="c263f-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="c263f-108">Pentru a afla mai multe, consultați [Configurarea setărilor politicii Microsoft Edge în Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="c263f-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
