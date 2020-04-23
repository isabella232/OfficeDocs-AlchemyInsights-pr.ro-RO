---
title: Depanarea sincronizării parolei
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732522"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="9fdad-102">Depanarea sincronizării parolei</span><span class="sxs-lookup"><span data-stu-id="9fdad-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="9fdad-103">Pentru a depana problemele în cazul în care nu există parole sincronizate cu Azure AD Conectați versiunea 1.1.614.0 sau o versiune ulterioară:</span><span class="sxs-lookup"><span data-stu-id="9fdad-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="9fdad-104">Deschideți o nouă sesiune Windows PowerShell pe serverul Azure AD Connect cu opțiunea **Executare ca Administrator.**</span><span class="sxs-lookup"><span data-stu-id="9fdad-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="9fdad-105">Executare **set-executionPolicy RemoteSigned** sau **Set-ExecutionPolicy nerestricționat**.</span><span class="sxs-lookup"><span data-stu-id="9fdad-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="9fdad-106">Porniți expertul Azure AD conecta.</span><span class="sxs-lookup"><span data-stu-id="9fdad-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="9fdad-107">Navigați la pagina **Activități suplimentare,** selectați **Depanare**și faceți clic pe **Următorul**.</span><span class="sxs-lookup"><span data-stu-id="9fdad-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="9fdad-108">În pagina Depanare, faceți clic pe **Lansare pentru a porni meniul de depanare** în PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9fdad-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="9fdad-109">În meniul principal, selectați **Depanare sincronizare parolă**.</span><span class="sxs-lookup"><span data-stu-id="9fdad-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="9fdad-110">În meniul sub, selectați **Sincronizare parolă nu funcționează deloc**.</span><span class="sxs-lookup"><span data-stu-id="9fdad-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="9fdad-111">**Înțelegerea rezultatelor activității de depanare**</span><span class="sxs-lookup"><span data-stu-id="9fdad-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="9fdad-112">Activitatea de depanare efectuează următoarele verificări:</span><span class="sxs-lookup"><span data-stu-id="9fdad-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="9fdad-113">Validează că caracteristica de sincronizare a parolei este activată pentru entitatea găzduită Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9fdad-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="9fdad-114">Validează că serverul Azure AD Connect nu este în modul de așteptare.</span><span class="sxs-lookup"><span data-stu-id="9fdad-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="9fdad-115">Pentru fiecare conector Active Directory local existent (care corespunde unei păduri Active Directory existente):</span><span class="sxs-lookup"><span data-stu-id="9fdad-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="9fdad-116">Validează că este activată caracteristica de sincronizare a parolei.</span><span class="sxs-lookup"><span data-stu-id="9fdad-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="9fdad-117">Caută evenimente de sincronizare a parolei în jurnalele de evenimente de eveniment aplicație Windows.</span><span class="sxs-lookup"><span data-stu-id="9fdad-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="9fdad-118">Pentru fiecare domeniu Active Directory sub conectorul Active Directory local:</span><span class="sxs-lookup"><span data-stu-id="9fdad-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="9fdad-119">Validează că domeniul este accesibil de pe serverul Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9fdad-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="9fdad-120">Validează că conturile active Directory Domain Services (AD DS) utilizate de conectorul Active Directory local are numele de utilizator, parola și permisiunile necesare pentru sincronizarea parolei.</span><span class="sxs-lookup"><span data-stu-id="9fdad-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="9fdad-121">Pentru mai multe ajutor depanarea sincronizarea parolei, consultați [Depanarea sincronizării parolei cu sincronizarea Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9fdad-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  