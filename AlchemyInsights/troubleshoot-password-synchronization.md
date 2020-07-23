---
title: Depanarea sincronizării parolei
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387889"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6ea84-102">Depanarea sincronizării parolei</span><span class="sxs-lookup"><span data-stu-id="6ea84-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6ea84-103">Pentru a depana problemele de sincronizare a parolei, începeți prin a utiliza această activitate de depanare AAD Connect pentru a determina de ce parolele nu se sincronizează.</span><span class="sxs-lookup"><span data-stu-id="6ea84-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="6ea84-104">Pentru a începe, [accesați Gestionare sincronizare directă](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="6ea84-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="6ea84-105">Deschideți o nouă sesiune Windows PowerShell pe serverul Azure AD Connect și selectați opțiunea **Executare ca administrator.**</span><span class="sxs-lookup"><span data-stu-id="6ea84-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="6ea84-106">Executați Set-ExecutionPolicy RemoteSigned sau Set-ExecutionPolicy Nerestricționat.</span><span class="sxs-lookup"><span data-stu-id="6ea84-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="6ea84-107">Porniți expertul Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6ea84-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="6ea84-108">Accesați pagina Activități suplimentare > **Depanare**  >  **următoare**.</span><span class="sxs-lookup"><span data-stu-id="6ea84-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="6ea84-109">Selectați **Lansare** pentru a deschide meniul de depanare PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6ea84-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="6ea84-110">Selectați **Depanare sincronizare parolă**.</span><span class="sxs-lookup"><span data-stu-id="6ea84-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="6ea84-111">Problema este, de obicei, că o parolă nu este sincronizat pentru un anumit cont de utilizator.</span><span class="sxs-lookup"><span data-stu-id="6ea84-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="6ea84-112">**Note** Sincronizarea parolei nu reușește dacă ultima sincronizare reușită a parolei a fost cu ceva timp în urmă.</span><span class="sxs-lookup"><span data-stu-id="6ea84-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="6ea84-113">Pentru mai mult ajutor pentru depanarea sincronizării parolei, consultați [Depanarea sincronizării hash a parolei cu sincronizarea Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6ea84-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>