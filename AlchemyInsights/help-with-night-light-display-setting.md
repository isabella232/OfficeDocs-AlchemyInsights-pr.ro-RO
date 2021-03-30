---
title: Ajutor pentru setarea pentru afișajul becului de noapte
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405178"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="24169-102">Ajutor pentru setarea pentru afișajul becului de noapte</span><span class="sxs-lookup"><span data-stu-id="24169-102">Help with the night light display setting</span></span>

<span data-ttu-id="24169-103">Pentru a afla mai multe despre setările de afișare pe timp de noapte, [consultați Setarea afișajului pe timp de noapte în Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="24169-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="24169-104">Dacă opțiunile pentru lumina de noapte sunt estompate în Setări, verificați driverul de afișare:</span><span class="sxs-lookup"><span data-stu-id="24169-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="24169-105">Faceți clic pe caseta de căutare din bara de activități **și tastați Manager** dispozitive , apoi **selectați Manager dispozitive** în rezultatele de căutare.</span><span class="sxs-lookup"><span data-stu-id="24169-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="24169-106">Extindeți **Plăci video**.</span><span class="sxs-lookup"><span data-stu-id="24169-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="24169-107">Din păcate, caracteristica de lumină de noapte nu este disponibilă dacă dispozitivul dvs. utilizează un driver DisplayLink sau un driver de afișare de bază.</span><span class="sxs-lookup"><span data-stu-id="24169-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="24169-108">Caracteristica lumină de noapte utilizează tehnologia grafică recentă, deci ar putea fi necesar să actualizați driverul de afișare:</span><span class="sxs-lookup"><span data-stu-id="24169-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="24169-109">Căutați actualizări, în Meniul **Pornire**  >  **actualizare setări**&  >  **Securitate**  >  **Windows Update** Căutare  >  **actualizări.**</span><span class="sxs-lookup"><span data-stu-id="24169-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="24169-110">SAU</span><span class="sxs-lookup"><span data-stu-id="24169-110">OR</span></span>

- <span data-ttu-id="24169-111">Vizitați site-ul web de asistență al producătorului de hardware pentru a descărca și instala manual cele mai recente drivere de afișare.</span><span class="sxs-lookup"><span data-stu-id="24169-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="24169-112">Resetați lumina de noapte din registry</span><span class="sxs-lookup"><span data-stu-id="24169-112">Reset night light in the registry</span></span>

<span data-ttu-id="24169-113">Dacă actualizarea driverului de afișare nu a funcționat, poate fi necesar să resetați lumina de noapte din registry.</span><span class="sxs-lookup"><span data-stu-id="24169-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="24169-114">**Atenție:** Acest pas de depanare este recomandat doar utilizatorilor avansați.</span><span class="sxs-lookup"><span data-stu-id="24169-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="24169-115">Pot apărea probleme grave dacă faceți modificări incorecte în registry.</span><span class="sxs-lookup"><span data-stu-id="24169-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="24169-116">Pentru protecție suplimentară, faceți backup pentru registry înainte de a-l modifica, astfel încât să îl puteți restaura dacă apar probleme.</span><span class="sxs-lookup"><span data-stu-id="24169-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="24169-117">În caseta de căutare, tastați **regedit**, apoi selectați **Registry Editor** în rezultatele căutării.</span><span class="sxs-lookup"><span data-stu-id="24169-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="24169-118">Accesați următoarea cheie de registry:</span><span class="sxs-lookup"><span data-stu-id="24169-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="24169-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="24169-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="24169-120">Exportați și ștergeți următoarea subcheie:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="24169-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="24169-121">Exportați și ștergeți următoarea subcheie:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="24169-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="24169-122">Reporniți Windows și verificați dacă sunt disponibile opțiunile pentru lumina de noapte.</span><span class="sxs-lookup"><span data-stu-id="24169-122">Restart Windows and verify if the night light options are available.</span></span>


