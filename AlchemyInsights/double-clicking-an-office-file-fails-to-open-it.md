---
title: Dacă faceți dublu clic pe un fișier Office, acesta nu reușește să-l deschidă
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814817"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="5e722-102">Dacă faceți dublu clic pe un fișier Office, acesta nu reușește să-l deschidă</span><span class="sxs-lookup"><span data-stu-id="5e722-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="5e722-103">După ce faceți dublu clic pe un fișier Office, este posibil să vedeți programul deschis, dar fișierul propriu-zis nu se deschide.</span><span class="sxs-lookup"><span data-stu-id="5e722-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="5e722-104">Sau este posibil să primiți eroarea: "A apărut o problemă la trimiterea comenzii la program."</span><span class="sxs-lookup"><span data-stu-id="5e722-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="5e722-105">Există multe cauze pentru acest lucru, dar cele mai comune două soluții sunt:</span><span class="sxs-lookup"><span data-stu-id="5e722-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="5e722-106">Din Excel, asigurați-vă că opțiunea DDE este debifată.</span><span class="sxs-lookup"><span data-stu-id="5e722-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="5e722-107">Opțiunea poate fi găsită creând un registru de lucru nou, apoi alegând **Fișier > Opțiuni > Complex**.</span><span class="sxs-lookup"><span data-stu-id="5e722-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="5e722-108">În **secțiunea General,** debifați **caseta de debifare Ignorare alte aplicații care utilizează Dynamic Data Exchange (DDE).**</span><span class="sxs-lookup"><span data-stu-id="5e722-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="5e722-109">Rulați o Reparare online pentru a restaura setările implicite.</span><span class="sxs-lookup"><span data-stu-id="5e722-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="5e722-110">Faceți clic pe butonul Start din Windows și căutați "Panou de control".</span><span class="sxs-lookup"><span data-stu-id="5e722-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="5e722-111">Deschideți Panoul **de control** și accesați Programe > Programe **și caracteristici.**</span><span class="sxs-lookup"><span data-stu-id="5e722-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="5e722-112">Apoi faceți clic dreapta **pe Microsoft Office [versiune]** și **alegeți Modificare > Reparare online.**</span><span class="sxs-lookup"><span data-stu-id="5e722-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="5e722-113">Dacă niciuna dintre aceste soluții nu funcționează, în articolul de asistență poate fi găsită o listă mai completă de soluții, dacă faceți dublu clic pe un fișier Office nu se poate [deschide.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="5e722-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
