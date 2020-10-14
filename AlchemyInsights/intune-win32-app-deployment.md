---
title: Implementarea aplicațiilor Win32 Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461877"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="59e2d-102">Implementarea aplicațiilor Win32 Intune</span><span class="sxs-lookup"><span data-stu-id="59e2d-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="59e2d-103">Microsoft Intune permite aplicațiilor Win32, inclusiv, dar fără a se limita la MSI și. EXE va fi implementat pe dispozitivele Windows 10.</span><span class="sxs-lookup"><span data-stu-id="59e2d-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="59e2d-104">Mecanismul de implementare utilizat necesită ca extensia de gestionare Intune (IME) să fie prezentă pe dispozitivul țintă.</span><span class="sxs-lookup"><span data-stu-id="59e2d-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="59e2d-105">IME va fi instalat automat ca urmare a țintirei unui script PowerShell sau a unei implementări de aplicații Win32 la un utilizator/dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="59e2d-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="59e2d-106">Există, de asemenea, un set de cerințe preliminare care trebuie îndeplinite pentru a implementa aplicații Win32 care includ:</span><span class="sxs-lookup"><span data-stu-id="59e2d-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="59e2d-107">Platforme acceptate: Windows 10 versiunea 1607 sau o versiune mai recentă (versiunile Enterprise, Pro și Education).</span><span class="sxs-lookup"><span data-stu-id="59e2d-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="59e2d-108">Arhitectură acceptată: x86 și x64.</span><span class="sxs-lookup"><span data-stu-id="59e2d-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="59e2d-109">Gestionarea dispozitivelor: Dan s-a alăturat și s-a înscris automat (inclusiv domeniul hibrid asociat și s-a înscris automat în Politica de grup).</span><span class="sxs-lookup"><span data-stu-id="59e2d-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="59e2d-110">Format pachet de aplicații:. fișier **intunewin**  pregătit de [instrumentul Microsoft Win32 Content Prep](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="59e2d-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="59e2d-111">Limite</span><span class="sxs-lookup"><span data-stu-id="59e2d-111">Limitations:</span></span>
    - <span data-ttu-id="59e2d-112">Dimensiunea maximă: 8GB.</span><span class="sxs-lookup"><span data-stu-id="59e2d-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="59e2d-113">Arhitectură neacceptată: ARMs.</span><span class="sxs-lookup"><span data-stu-id="59e2d-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="59e2d-114">Revizuiți documentul "[adăugarea, atribuirea și monitorizarea unei aplicații Win32 în Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" pentru informații legate de acești pași.</span><span class="sxs-lookup"><span data-stu-id="59e2d-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="59e2d-115">Detalii despre depanarea implementării aplicațiilor pe Windows, inclusiv aplicațiile Win32 pot fi revizuite în următoarele documente</span><span class="sxs-lookup"><span data-stu-id="59e2d-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="59e2d-116">Depanarea problemelor de instalare a aplicațiilor</span><span class="sxs-lookup"><span data-stu-id="59e2d-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="59e2d-117">Depanarea aplicațiilor Win32</span><span class="sxs-lookup"><span data-stu-id="59e2d-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)