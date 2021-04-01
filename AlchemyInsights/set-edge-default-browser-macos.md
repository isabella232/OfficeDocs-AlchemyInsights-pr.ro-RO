---
title: Setați Microsoft Edge ca browser implicit pe un dispozitiv macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491812"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="d9f3b-102">Setați Microsoft Edge ca browser implicit pe un dispozitiv macOS</span><span class="sxs-lookup"><span data-stu-id="d9f3b-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="d9f3b-103">Utilizați una dintre aceste două metode pentru a seta Microsoft Edge ca browser implicit:</span><span class="sxs-lookup"><span data-stu-id="d9f3b-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="d9f3b-104">Metoda 1: Dați un flash dispozitivului cu o imagine cu macOS, unde Microsoft Edge a fost setat deja ca browser implicit.</span><span class="sxs-lookup"><span data-stu-id="d9f3b-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="d9f3b-105">Metoda 2: Setați politica DefaultBrowserSettingEnabled pentru a-i solicita utilizatorului să setați Microsoft Edge ca browser implicit.</span><span class="sxs-lookup"><span data-stu-id="d9f3b-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="d9f3b-106">Oricare dintre metode îi permite unui utilizator să modifice browserul implicit.</span><span class="sxs-lookup"><span data-stu-id="d9f3b-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="d9f3b-107">Din acest motiv, vă recomandăm să implementați politica DefaultBrowserSettingEnabled, chiar dacă s-a utilizat metoda 1.</span><span class="sxs-lookup"><span data-stu-id="d9f3b-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="d9f3b-108">Dacă un utilizator modifică browserul implicit după ce politica este implementată, politica solicită utilizatorului să seteze browserul implicit înapoi la Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d9f3b-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
