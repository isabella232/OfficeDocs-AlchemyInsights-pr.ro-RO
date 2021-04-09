---
title: Remedierea 0x8004de40 eroare în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649760"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="f4294-102">Remedierea 0x8004de40 eroare în OneDrive</span><span class="sxs-lookup"><span data-stu-id="f4294-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="f4294-103">Dacă rulați Windows 7 și primiți această eroare, Actualizați pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)protocoale sigure implicite în WinHTTP în Windows .</span><span class="sxs-lookup"><span data-stu-id="f4294-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="f4294-104">Dacă rulați Windows 10 și primiți o eroare 0x8004de40 cu OneDrive:</span><span class="sxs-lookup"><span data-stu-id="f4294-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="f4294-105">Reporniți computerul afectat în timp ce sunteți conectat la domeniul Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="f4294-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="f4294-106">Dacă o repornire nu remediază problema, anulați-vă și reasezați-vă dispozitivul din Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4294-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="f4294-107">**Notă:** Ar trebui să vă a afla în rețeaua de corporație în timp ce efectuați acești pași.</span><span class="sxs-lookup"><span data-stu-id="f4294-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="f4294-108">Nu efectuați acești pași atunci când nu sunteți conectat la infrastructura de corporație (de exemplu, în timpul călătoriilor).</span><span class="sxs-lookup"><span data-stu-id="f4294-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="f4294-109">Deschideți o linie de comandă cu drepturi înălțimii selectând **Start,** faceți clic **dreapta pe Linie de** comandă, apoi **selectați Rulare ca administrator**.</span><span class="sxs-lookup"><span data-stu-id="f4294-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="f4294-110">Tastați *dsregcmd /leave și* apăsați **pe Enter**.</span><span class="sxs-lookup"><span data-stu-id="f4294-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="f4294-111">Când terminați, tastați *dsregcmd /join și* apăsați pe **Enter**.</span><span class="sxs-lookup"><span data-stu-id="f4294-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="f4294-112">Când terminați, închideți linia de comandă.</span><span class="sxs-lookup"><span data-stu-id="f4294-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="f4294-113">Reporniți computerul și conectați-vă la OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f4294-113">Reboot the computer, and log into OneDrive.</span></span>