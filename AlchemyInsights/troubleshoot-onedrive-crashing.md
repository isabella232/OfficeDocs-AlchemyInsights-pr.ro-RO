---
title: Depanarea căderilor OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749166"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="a731c-102">Depanarea căderilor OneDrive</span><span class="sxs-lookup"><span data-stu-id="a731c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="a731c-103">Dacă OneDrive se blochează în mod repetat, încercați acești pași de depanare:</span><span class="sxs-lookup"><span data-stu-id="a731c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="a731c-104">**Asigurați-vă că cheile de registry nu sunt setate:**</span><span class="sxs-lookup"><span data-stu-id="a731c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="a731c-105">Utilizând Registry Editor, navigați la HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="a731c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="a731c-106">Dacă DisableFileSyncNGSC este prezent și setat la 1, deschideți cheia și modificați valoarea la 0.</span><span class="sxs-lookup"><span data-stu-id="a731c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="a731c-107">Lansați manual OneDrive mergând la Start</span><span class="sxs-lookup"><span data-stu-id="a731c-107">Manually launch OneDrive by going to Start</span></span> ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a731c-109">, tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a731c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a731c-110">**Reinițializare OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="a731c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="a731c-111">Note:</span><span class="sxs-lookup"><span data-stu-id="a731c-111">Notes:</span></span>

- <span data-ttu-id="a731c-112">Resetarea OneDrive deconectează toate conexiunile de sincronizare existente (inclusiv OneDrive-ul personal, dacă este configurat).</span><span class="sxs-lookup"><span data-stu-id="a731c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="a731c-113">Nu veți pierde fișiere sau date prin resetarea OneDrive pe computer.</span><span class="sxs-lookup"><span data-stu-id="a731c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="a731c-114">**Pentru a reseta OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="a731c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="a731c-115">Deschideți un dialog Executare apăsând tasta Windows și R.</span><span class="sxs-lookup"><span data-stu-id="a731c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="a731c-116">Tastați %localappdata%\Microsoft\OneDrive\onedrive.exe /reset și apăsați OK.</span><span class="sxs-lookup"><span data-stu-id="a731c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="a731c-117">Este posibil ca o fereastră Comandă să apară pentru scurt timp.</span><span class="sxs-lookup"><span data-stu-id="a731c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="a731c-118">Lansați manual OneDrive mergând la Start</span><span class="sxs-lookup"><span data-stu-id="a731c-118">Manually launch OneDrive by going to Start</span></span> ![Apăsați tasta Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="a731c-120">, tastați OneDrive în caseta de căutare, apoi faceți clic pe aplicația desktop OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a731c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="a731c-121">Note:</span><span class="sxs-lookup"><span data-stu-id="a731c-121">Notes:</span></span>

- <span data-ttu-id="a731c-122">Dacă ați ales să sincronizați doar unele foldere înainte de resetare, va trebui să faceți acest lucru din nou după terminarea sincronizării.</span><span class="sxs-lookup"><span data-stu-id="a731c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="a731c-123">Citiți [Alegeți ce foldere OneDrive să sincronizați la computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)pentru mai multe   informații.</span><span class="sxs-lookup"><span data-stu-id="a731c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="a731c-124">Va trebui să finalizați acest lucru pentru OneDrive și OneDrive pentru business personale.</span><span class="sxs-lookup"><span data-stu-id="a731c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>