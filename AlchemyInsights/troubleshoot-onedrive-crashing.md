---
title: Depanarea căderilor OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665010"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="0b6b7-102">Depanarea căderilor OneDrive</span><span class="sxs-lookup"><span data-stu-id="0b6b7-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="0b6b7-103">Dacă OneDrive se defectează în mod repetat, încercați acești pași de depanare:</span><span class="sxs-lookup"><span data-stu-id="0b6b7-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="0b6b7-104">**Asigurați-vă că nu sunt setate cheile de registry:**</span><span class="sxs-lookup"><span data-stu-id="0b6b7-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="0b6b7-105">Utilizarea Registry Editor, navigați la HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="0b6b7-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="0b6b7-106">Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="0b6b7-107">Lansați manual OneDrive accesând Start</span><span class="sxs-lookup"><span data-stu-id="0b6b7-107">Manually launch OneDrive by going to Start</span></span> ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="0b6b7-109">, tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="0b6b7-110">**Reinițializați OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="0b6b7-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="0b6b7-111">Note</span><span class="sxs-lookup"><span data-stu-id="0b6b7-111">Notes:</span></span>

- <span data-ttu-id="0b6b7-112">Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv OneDrive personal, dacă este configurat).</span><span class="sxs-lookup"><span data-stu-id="0b6b7-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="0b6b7-113">Nu veți pierde fișiere sau date prin reinițializarea OneDrive pe computer.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="0b6b7-114">**Pentru a reseta OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="0b6b7-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="0b6b7-115">Deschideți o casetă de dialog rulare apăsând tasta Windows și R.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="0b6b7-116">Tastați% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset și apăsați pe OK.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="0b6b7-117">O fereastră de comandă poate apărea pe scurt.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="0b6b7-118">Lansați manual OneDrive accesând Start</span><span class="sxs-lookup"><span data-stu-id="0b6b7-118">Manually launch OneDrive by going to Start</span></span> ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="0b6b7-120">, tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="0b6b7-121">Note</span><span class="sxs-lookup"><span data-stu-id="0b6b7-121">Notes:</span></span>

- <span data-ttu-id="0b6b7-122">Dacă ați ales să sincronizați doar unele foldere înainte de resetare, va trebui să faceți acest lucru din nou după ce sincronizarea s-a finalizat.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="0b6b7-123">Citiți [Alegeți ce foldere OneDrive să se sincronizeze cu computerul](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="0b6b7-124">Va trebui să terminați acest lucru pentru OneDrive personal și OneDrive pentru Business.</span><span class="sxs-lookup"><span data-stu-id="0b6b7-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>