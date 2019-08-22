---
title: Depanarea sincronizarea parolelor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533819"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c4423-102">Depanarea sincronizarea parolelor</span><span class="sxs-lookup"><span data-stu-id="c4423-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c4423-103">Pentru a depana probleme în cazul în care parolele nu sunt sincronizate cu Azure AD conecta versiunea 1.1.614.0 sau o versiune ulterioară:</span><span class="sxs-lookup"><span data-stu-id="c4423-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="c4423-104">Deschideti o noua sesiune de Windows PowerShell pe serverul AD Azure Connect cu opţiunea de **a alerga as Administrator** .</span><span class="sxs-lookup"><span data-stu-id="c4423-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c4423-105">Executați **Set-ExecutionPolicy RemoteSigned** sau **Set-ExecutionPolicy nerestricționată**.</span><span class="sxs-lookup"><span data-stu-id="c4423-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="c4423-106">Porni Expertul Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c4423-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c4423-107">Navigați la **Sarcini suplimentare** , selectaţi **Depanarea**şi faceţi clic pe **Următorul**.</span><span class="sxs-lookup"><span data-stu-id="c4423-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="c4423-108">Pagina de depanare, faceţi clic pe meniul de **lansare pentru a începe depanarea** în PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c4423-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="c4423-109">În meniul principal, selectaţi **Depanarea sincronizarea parolelor**.</span><span class="sxs-lookup"><span data-stu-id="c4423-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="c4423-110">În sub-meniu, selectaţi **sincronizarea parolelor nu funcţionează deloc**.</span><span class="sxs-lookup"><span data-stu-id="c4423-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="c4423-111">**Intelege rezultatele misiunii depanare**</span><span class="sxs-lookup"><span data-stu-id="c4423-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="c4423-112">Sarcina depanare efectuează următoarele verificări:</span><span class="sxs-lookup"><span data-stu-id="c4423-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="c4423-113">Validează că funcţia de sincronizare parolare este activată pentru chiriaşul dumneavoastră azuriu AD.</span><span class="sxs-lookup"><span data-stu-id="c4423-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="c4423-114">Validează că Azure AD Connect server nu este în modul de așteptare.</span><span class="sxs-lookup"><span data-stu-id="c4423-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="c4423-115">Pentru fiecare existente local Active Directory connector, (care corespunde la o pădure Active Directory existente):</span><span class="sxs-lookup"><span data-stu-id="c4423-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="c4423-116">Validează faptul că este activată caracteristica de sincronizare parola.</span><span class="sxs-lookup"><span data-stu-id="c4423-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="c4423-117">Căutările pentru parola sincronizare emoţie evenimente în jurnalele de evenimente de aplicaţie Windows.</span><span class="sxs-lookup"><span data-stu-id="c4423-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="c4423-118">Pentru fiecare domeniu Active Directory în conectorul de Active Directory local:</span><span class="sxs-lookup"><span data-stu-id="c4423-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="c4423-119">Validează că domeniul este accesibilă de pe serverul AD Azure Connect.</span><span class="sxs-lookup"><span data-stu-id="c4423-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="c4423-120">Validează că serviciile de domeniu Active Directory (AD DS) conturile utilizate de conectorul de Active Directory local are corect numele de utilizator, parola şi permisiunile necesare pentru sincronizarea parolelor.</span><span class="sxs-lookup"><span data-stu-id="c4423-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="c4423-121">Pentru mai mult ajutor parola sincronizare de depanare, consultaţi [Depanarea sincronizarea parolelor cu Azure AD conecta sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c4423-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  