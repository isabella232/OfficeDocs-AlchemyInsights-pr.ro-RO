---
title: Rulați Diagnostice memorie Windows în Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826679"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="b6515-102">Rulați Diagnostice memorie Windows în Windows 10</span><span class="sxs-lookup"><span data-stu-id="b6515-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="b6515-103">Dacă Windows și aplicațiile de pe PC se blochează, îngheașează sau acționează într-un mod instabil, este posibil să aveți o problemă cu memoria PC-ului (RAM).</span><span class="sxs-lookup"><span data-stu-id="b6515-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="b6515-104">Puteți rula Diagnostic memorie Windows pentru a căuta probleme cu RAM-ul PC-ului.</span><span class="sxs-lookup"><span data-stu-id="b6515-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="b6515-105">În caseta de căutare din bara de activități, tastați **diagnostic de memorie**, apoi selectați Diagnosticare memorie **Windows**.</span><span class="sxs-lookup"><span data-stu-id="b6515-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="b6515-106">Pentru a rula diagnosticarea, PC-ul trebuie să repornească.</span><span class="sxs-lookup"><span data-stu-id="b6515-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="b6515-107">Aveți opțiunea să reporniți imediat (salvați-vă lucrul și închideți mai întâi documentele și mesajele de e-mail deschise) sau programați diagnosticarea să ruleze automat data următoare când PC-ul repornește:</span><span class="sxs-lookup"><span data-stu-id="b6515-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnosticare memorie Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="b6515-109">Atunci când PC-ul repornește, **Instrumentul de diagnosticare a memoriei Windows** va rula automat.</span><span class="sxs-lookup"><span data-stu-id="b6515-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="b6515-110">Starea și progresul se vor afișa pe măsură ce rulează diagnosticele și veți avea opțiunea de a anula diagnosticele apăsând tasta **ESC** pe tastatură.</span><span class="sxs-lookup"><span data-stu-id="b6515-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="b6515-111">Atunci când diagnosticele sunt finalizate, Windows va porni normal.</span><span class="sxs-lookup"><span data-stu-id="b6515-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="b6515-112">Imediat după repornire, atunci când apare Desktopul,  va apărea o notificare (lângă pictograma Acțiuni din bara de activități), pentru a indica dacă s-au găsit erori de memorie.</span><span class="sxs-lookup"><span data-stu-id="b6515-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="b6515-113">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="b6515-113">For example:</span></span>

<span data-ttu-id="b6515-114">Iată pictograma Acțiuni:</span><span class="sxs-lookup"><span data-stu-id="b6515-114">Here's the Action Center icon:</span></span> ![Pictograma Acțiuni](media/action-center-icon.png) 

<span data-ttu-id="b6515-116">Și un exemplu de notificare:</span><span class="sxs-lookup"><span data-stu-id="b6515-116">And a sample notification:</span></span> ![Nicio eroare de memorie](media/no-memory-errors.png)

<span data-ttu-id="b6515-118">Dacă nu vedeți notificarea,  puteți selecta pictograma Acțiuni  de pe bara de activități pentru a afișa Acțiuni și a vedea o listă de notificări prin care se poate defila.</span><span class="sxs-lookup"><span data-stu-id="b6515-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="b6515-119">Pentru a revizui informațiile detaliate, **tastați eveniment** în caseta de căutare din bara de activități, apoi selectați **Vizualizator evenimente**.</span><span class="sxs-lookup"><span data-stu-id="b6515-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="b6515-120">În panoul **din stânga** al Vizualizatorului de evenimente, navigați la **Jurnale Windows > Sistem**.</span><span class="sxs-lookup"><span data-stu-id="b6515-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="b6515-121">În panoul din dreapta, scanați lista în timp ce priviți coloana **Sursă,** până când vedeți evenimente cu valoarea sursă **MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="b6515-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="b6515-122">Evidențiați fiecare astfel de eveniment și vedeți informațiile despre rezultate în caseta de **sub fila General** de sub listă.</span><span class="sxs-lookup"><span data-stu-id="b6515-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
