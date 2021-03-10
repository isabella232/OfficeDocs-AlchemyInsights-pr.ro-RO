---
title: Depanarea problemelor de instalare MDATP pe un Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696093"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="7db18-102">Depanarea problemelor de instalare MDATP pe un Mac</span><span class="sxs-lookup"><span data-stu-id="7db18-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="7db18-103">Dacă instalarea manuală nu reușește, pagina **Rezumat** a expertului de instalare afișează următoarea eroare:</span><span class="sxs-lookup"><span data-stu-id="7db18-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="7db18-104">"A apărut o eroare în timpul instalării.</span><span class="sxs-lookup"><span data-stu-id="7db18-104">"An error occurred during installation.</span></span> <span data-ttu-id="7db18-105">Programul de instalare a întâlnit o eroare care a determinat instalarea să nu reușească.</span><span class="sxs-lookup"><span data-stu-id="7db18-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="7db18-106">Contactați producătorul software-ului pentru asistență. "</span><span class="sxs-lookup"><span data-stu-id="7db18-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="7db18-107">Pentru implementările MDM, pagina afișează și o eroare generică de instalare.</span><span class="sxs-lookup"><span data-stu-id="7db18-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="7db18-108">Deși nu se afișează erorile exacte pentru utilizatorii finali, păstrăm un fișier jurnal cu progresul instalării, în **/Library/logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="7db18-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="7db18-109">Fiecare sesiune de instalare se adaugă la acest fișier jurnal.</span><span class="sxs-lookup"><span data-stu-id="7db18-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="7db18-110">Pentru a afișa numai ultima sesiune de instalare, utilizați `sed` .</span><span class="sxs-lookup"><span data-stu-id="7db18-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="7db18-111">Pentru a afla mai multe, consultați [Depanarea problemelor de instalare pentru Microsoft Defender ATP pentru Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="7db18-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
