---
title: Depanarea sincronizării parolei
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664938"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6d060-102">Depanarea sincronizării parolei</span><span class="sxs-lookup"><span data-stu-id="6d060-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6d060-103">Pentru a depana problemele de sincronizare a parolei, începeți prin a utiliza această activitate de depanare AAD Connect pentru a determina de ce parolele nu se sincronizează.</span><span class="sxs-lookup"><span data-stu-id="6d060-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="6d060-104">Pentru a începe, accesați [gestionare sincronizare directă](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="6d060-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="6d060-105">Deschideți o nouă sesiune Windows PowerShell pe serverul Azure AD Connect și selectați opțiunea **Executare ca administrator** .</span><span class="sxs-lookup"><span data-stu-id="6d060-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="6d060-106">Rulează set-ExecutionPolicy RemoteSigned sau set-ExecutionPolicy nerestricționate.</span><span class="sxs-lookup"><span data-stu-id="6d060-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="6d060-107">Porniți Expertul Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6d060-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="6d060-108">Accesați pagina activități suplimentare > depanare în **Troubleshoot**  >  **continuare**.</span><span class="sxs-lookup"><span data-stu-id="6d060-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="6d060-109">Selectați **lansare** pentru a deschide meniul depanare PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6d060-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="6d060-110">Selectați **depanați sincronizarea parolelor**.</span><span class="sxs-lookup"><span data-stu-id="6d060-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="6d060-111">Problema este, de obicei, că o parolă nu este sincronizată pentru un anumit cont de utilizator.</span><span class="sxs-lookup"><span data-stu-id="6d060-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="6d060-112">**Note** Sincronizarea parolelor nu reușește dacă Ultima sincronizare cu parolă reușită a fost acum ceva timp.</span><span class="sxs-lookup"><span data-stu-id="6d060-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="6d060-113">Pentru mai mult ajutor la depanarea sincronizării parolei, consultați [Depanarea sincronizării hash a parolei cu sincronizarea AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6d060-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>