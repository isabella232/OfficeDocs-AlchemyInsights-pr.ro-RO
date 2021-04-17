---
title: Depanarea problemelor cu OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826211"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="64874-102">Depanarea problemelor cu OneDrive</span><span class="sxs-lookup"><span data-stu-id="64874-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="64874-103">Dacă OneDrive se blochează în mod repetat, încercați acești pași de depanare:</span><span class="sxs-lookup"><span data-stu-id="64874-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="64874-104">**Asigurați-vă că nu sunt setate chei de registry:**</span><span class="sxs-lookup"><span data-stu-id="64874-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="64874-105">Utilizând Registry Editor, navigați la HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="64874-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="64874-106">Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.</span><span class="sxs-lookup"><span data-stu-id="64874-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="64874-107">Lansați manual OneDrive, în start</span><span class="sxs-lookup"><span data-stu-id="64874-107">Manually launch OneDrive by going to Start</span></span> ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="64874-109">, tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="64874-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="64874-110">**Resetați OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="64874-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="64874-111">Note:</span><span class="sxs-lookup"><span data-stu-id="64874-111">Notes:</span></span>

- <span data-ttu-id="64874-112">Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv contul OneDrive personal, dacă este configurat).</span><span class="sxs-lookup"><span data-stu-id="64874-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="64874-113">Nu veți pierde fișiere sau date în cazul resetării OneDrive pe computer.</span><span class="sxs-lookup"><span data-stu-id="64874-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="64874-114">**Pentru a reseta OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="64874-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="64874-115">Deschideți o casetă de dialog Executare, apăsând tasta Windows și R.</span><span class="sxs-lookup"><span data-stu-id="64874-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="64874-116">Tastați %localappdata%\Microsoft\OneDrive\onedrive.exe /reset și apăsați OK.</span><span class="sxs-lookup"><span data-stu-id="64874-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="64874-117">Poate apărea o fereastră de comandă pentru un timp scurt.</span><span class="sxs-lookup"><span data-stu-id="64874-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="64874-118">Lansați manual OneDrive, în start</span><span class="sxs-lookup"><span data-stu-id="64874-118">Manually launch OneDrive by going to Start</span></span> ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="64874-120">, tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="64874-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="64874-121">Note:</span><span class="sxs-lookup"><span data-stu-id="64874-121">Notes:</span></span>

- <span data-ttu-id="64874-122">Dacă ați ales să sincronizați doar unele foldere înainte de a reseta, va trebui să faceți acest lucru din nou după ce se încheie sincronizarea.</span><span class="sxs-lookup"><span data-stu-id="64874-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="64874-123">Citiți [Alegeți ce foldere OneDrive să se sincronizeze cu computerul dvs.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="64874-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="64874-124">Va trebui să faceți acest lucru pentru contul OneDrive personal și pentru OneDrive pentru business.</span><span class="sxs-lookup"><span data-stu-id="64874-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>