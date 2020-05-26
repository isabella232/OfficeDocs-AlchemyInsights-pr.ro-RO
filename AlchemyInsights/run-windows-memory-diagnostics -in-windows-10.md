---
title: Executarea diagnosticelor de memorie Windows în Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357784"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="88118-102">Executarea diagnosticelor de memorie Windows în Windows 10</span><span class="sxs-lookup"><span data-stu-id="88118-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="88118-103">Dacă Windows și aplicațiile de pe PC se blochează, înghedează sau acționează într-un mod instabil, este posibil să aveți o problemă cu memoria PC-ului (RAM).</span><span class="sxs-lookup"><span data-stu-id="88118-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="88118-104">Aveți posibilitatea să executați Windows Memory Diagnostic pentru a căuta probleme cu memoria RAM a PC-ului.</span><span class="sxs-lookup"><span data-stu-id="88118-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="88118-105">În caseta de căutare din bara de activități, tastați **diagnosticare memorie**, apoi selectați Diagnosticare **memorie Windows**.</span><span class="sxs-lookup"><span data-stu-id="88118-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="88118-106">Pentru a executa diagnosticarea, PC-ul trebuie să repornească.</span><span class="sxs-lookup"><span data-stu-id="88118-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="88118-107">Aveți opțiunea de a reporni imediat (vă rugăm să salvați lucrul și să închideți mai întâi documentele deschise și e-mailurile) sau să programați diagnosticarea să ruleze automat data viitoare când PC-ul repornește:</span><span class="sxs-lookup"><span data-stu-id="88118-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnosticare memorie Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="88118-109">Când PC-ul repornește, **instrumentul de diagnosticare a memoriei Windows** se va executa automat.</span><span class="sxs-lookup"><span data-stu-id="88118-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="88118-110">Starea și progresul vor fi afișate pe măsură ce se execută diagnosticarea și aveți opțiunea de a anula diagnosticarea apăsând tasta **ESC** de pe tastatură.</span><span class="sxs-lookup"><span data-stu-id="88118-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="88118-111">Când diagnosticarea este finalizată, Windows va porni normal.</span><span class="sxs-lookup"><span data-stu-id="88118-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="88118-112">Imediat după repornire, când apare Desktopul, va apărea o notificare (lângă pictograma **Centru de acțiune** din bara de activități), pentru a indica dacă s-au găsit erori de memorie.</span><span class="sxs-lookup"><span data-stu-id="88118-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="88118-113">De exemplu:</span><span class="sxs-lookup"><span data-stu-id="88118-113">For example:</span></span>

<span data-ttu-id="88118-114">Iată pictograma Centru de acțiune:</span><span class="sxs-lookup"><span data-stu-id="88118-114">Here's the Action Center icon:</span></span> ![Pictograma Centru de acțiune](media/action-center-icon.png) 

<span data-ttu-id="88118-116">Și o notificare eșantion:</span><span class="sxs-lookup"><span data-stu-id="88118-116">And a sample notification:</span></span> ![Fără erori de memorie](media/no-memory-errors.png)

<span data-ttu-id="88118-118">Dacă ați pierdut notificarea, puteți selecta pictograma **Centru de acțiune** din bara de activități pentru a afișa Centrul de **acțiune** și a vedea o listă de notificări derulantă.</span><span class="sxs-lookup"><span data-stu-id="88118-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="88118-119">Pentru a revizui informații detaliate, tastați **eveniment** în caseta de căutare din bara de activități, apoi selectați **Vizualizator evenimente**.</span><span class="sxs-lookup"><span data-stu-id="88118-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="88118-120">În panoul din stânga vizualizatorului de **evenimente,** navigați la **Windows Logs > System**.</span><span class="sxs-lookup"><span data-stu-id="88118-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="88118-121">În panoul din dreapta, scanați lista în timp ce căutați coloana **Sursă,** până când vedeți evenimente cu valoare sursă **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="88118-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="88118-122">Evidențiați fiecare astfel de eveniment și vedeți informațiile despre rezultate în caseta de sub fila **General** de sub listă.</span><span class="sxs-lookup"><span data-stu-id="88118-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
