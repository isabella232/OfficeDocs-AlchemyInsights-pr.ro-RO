---
title: Setarea ClientAccessServerEnabled la True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525964"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="e782a-102">Setarea ClientAccessServerEnabled la True</span><span class="sxs-lookup"><span data-stu-id="e782a-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="e782a-103">Dacă nu puteți deschide un mesaj de e-mail criptat și vedeți în schimb o atașare **rpmsg** , efectuați pașii următori:</span><span class="sxs-lookup"><span data-stu-id="e782a-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="e782a-104">Conectați-vă la Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e782a-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="e782a-105">Pentru a vă conecta la Exchange Online PowerShell, trebuie să vă conectați utilizând un cont de administrator global sau Exchange.</span><span class="sxs-lookup"><span data-stu-id="e782a-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="e782a-106">un.</span><span class="sxs-lookup"><span data-stu-id="e782a-106">a.</span></span> <span data-ttu-id="e782a-107">Deschideți Windows PowerShell, apoi rulează următoarea comandă: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="e782a-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="e782a-108">b.</span><span class="sxs-lookup"><span data-stu-id="e782a-108">b.</span></span> <span data-ttu-id="e782a-109">În caseta de dialog **solicitare de acreditare Windows PowerShell** , introduceți contul de la locul de muncă sau de la școală și parola, c.</span><span class="sxs-lookup"><span data-stu-id="e782a-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="e782a-110">Faceți clic pe **OK**.</span><span class="sxs-lookup"><span data-stu-id="e782a-110">Click **OK**.</span></span> 

2. <span data-ttu-id="e782a-111">Rulează următoarea comandă pentru a crea o sesiune nouă:</span><span class="sxs-lookup"><span data-stu-id="e782a-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="e782a-112">un.</span><span class="sxs-lookup"><span data-stu-id="e782a-112">a.</span></span> <span data-ttu-id="e782a-113">Rulați următoarea comandă:</span><span class="sxs-lookup"><span data-stu-id="e782a-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="e782a-114">`Get-IRMConfiguration`Comanda rulare.</span><span class="sxs-lookup"><span data-stu-id="e782a-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="e782a-115">Verificați setarea **ClientAccessServerEnabled** .</span><span class="sxs-lookup"><span data-stu-id="e782a-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="e782a-116">un.</span><span class="sxs-lookup"><span data-stu-id="e782a-116">a.</span></span> <span data-ttu-id="e782a-117">Dacă setarea **ClientAccessServerEnabled** este setată la **false**, rulează următorul cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="e782a-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="e782a-118">Închideți întotdeauna sesiunea PowerShell cu următoarea comandă: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="e782a-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="e782a-119">Pentru mai multe informații, consultați [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="e782a-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

