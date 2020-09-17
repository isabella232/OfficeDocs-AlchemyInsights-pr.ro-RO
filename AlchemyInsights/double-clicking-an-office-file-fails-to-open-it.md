---
title: Dacă faceți dublu clic pe un fișier Office nu reușește să îl deschidă
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812091"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="e2774-102">Dacă faceți dublu clic pe un fișier Office nu reușește să îl deschidă</span><span class="sxs-lookup"><span data-stu-id="e2774-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="e2774-103">După ce faceți dublu clic pe un fișier Office, este posibil să vedeți programul deschis, dar fișierul propriu-zis nu se deschide.</span><span class="sxs-lookup"><span data-stu-id="e2774-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="e2774-104">Sau este posibil să primiți eroarea: "a apărut o problemă la trimiterea comenzii la program".</span><span class="sxs-lookup"><span data-stu-id="e2774-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="e2774-105">Există multe cauze pentru aceasta, dar cele mai comune două soluții sunt:</span><span class="sxs-lookup"><span data-stu-id="e2774-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="e2774-106">Din Excel, asigurați-vă că opțiunea DDE este debifată.</span><span class="sxs-lookup"><span data-stu-id="e2774-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="e2774-107">Opțiunea poate fi găsită creând un registru de lucru nou, apoi alegând **opțiuni > fișier > complex**.</span><span class="sxs-lookup"><span data-stu-id="e2774-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="e2774-108">În secțiunea **General** , debifați **ignorarea altor aplicații care utilizează Dynamic Data Exchange (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="e2774-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="e2774-109">Rularea unei reparații online pentru a restaura setările implicite.</span><span class="sxs-lookup"><span data-stu-id="e2774-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="e2774-110">Faceți clic pe butonul Start din Windows și căutați "panou de control".</span><span class="sxs-lookup"><span data-stu-id="e2774-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="e2774-111">Deschideți **panoul de control**și accesați **programe > programe și caracteristici**.</span><span class="sxs-lookup"><span data-stu-id="e2774-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="e2774-112">Apoi faceți clic dreapta pe **Microsoft Office [versiune]** și alegeți **modificare > reparare online**.</span><span class="sxs-lookup"><span data-stu-id="e2774-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="e2774-113">Dacă niciuna dintre aceste soluții nu funcționează, se poate găsi o listă de soluții mai completă în articolul de asistență, [făcând dublu clic pe un fișier Office nu reușește să îl deschidă](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="e2774-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
