---
title: Eliminarea serviciului de fundal pentru Microsoft Search în Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816335"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="e32c4-102">Eliminarea serviciului de fundal pentru Microsoft Search în Bing</span><span class="sxs-lookup"><span data-stu-id="e32c4-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="e32c4-103">Pentru a elimina serviciul de fundal pentru Microsoft Search în Bing, puteți încerca următoarele căi de atac:</span><span class="sxs-lookup"><span data-stu-id="e32c4-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="e32c4-104">Pentru a reveni la setările motorului de căutare inițial, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="e32c4-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="e32c4-105">un.</span><span class="sxs-lookup"><span data-stu-id="e32c4-105">a.</span></span> <span data-ttu-id="e32c4-106">Comutați opțiunea **Utilizați Bing ca motor de [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) căutare implicit dezactivat**.</span><span class="sxs-lookup"><span data-stu-id="e32c4-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="e32c4-107">b.</span><span class="sxs-lookup"><span data-stu-id="e32c4-107">b.</span></span> <span data-ttu-id="e32c4-108">[Accesați centrul de administrare Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) și debifați setarea care afectează toți utilizatorii din organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="e32c4-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="e32c4-109">Pentru a elimina serviciul de fundal de pe un dispozitiv individual, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="e32c4-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="e32c4-110">un.</span><span class="sxs-lookup"><span data-stu-id="e32c4-110">a.</span></span> <span data-ttu-id="e32c4-111">Alegeți **Panou de Control > programe > programe și caracteristici**.</span><span class="sxs-lookup"><span data-stu-id="e32c4-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="e32c4-112">b.</span><span class="sxs-lookup"><span data-stu-id="e32c4-112">b.</span></span> <span data-ttu-id="e32c4-113">Faceți clic cu butonul din dreapta pe **Microsoft Search în Bing** sub lista de programe instalate, apoi faceți clic pe **Dezinstalare**.</span><span class="sxs-lookup"><span data-stu-id="e32c4-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="e32c4-114">Pentru a elimina serviciul de fundal de pe mai multe dispozitive din organizație, conectați-vă ca administrator și derulează următoarea comandă într-un script:</span><span class="sxs-lookup"><span data-stu-id="e32c4-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
