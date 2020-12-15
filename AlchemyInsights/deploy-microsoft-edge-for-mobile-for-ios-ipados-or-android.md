---
title: Implementarea Microsoft Edge pentru dispozitive mobile pentru iOS/iPadOS sau Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679941"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="86b74-102">Implementarea Microsoft Edge pentru dispozitive mobile pentru iOS/iPadOS sau Android</span><span class="sxs-lookup"><span data-stu-id="86b74-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="86b74-103">Scenariul ghidat rezumat mai jos vă va ajuta să atribuiți Microsoft Edge utilizatorilor de dispozitive iOS, iPadOS și Android.</span><span class="sxs-lookup"><span data-stu-id="86b74-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="86b74-104">După ce terminați acești pași, politicile Microsoft Intune vor activa următoarele caracteristici Microsoft Edge pentru Business:</span><span class="sxs-lookup"><span data-stu-id="86b74-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="86b74-105">Identitate dublă</span><span class="sxs-lookup"><span data-stu-id="86b74-105">Dual identity</span></span>
- <span data-ttu-id="86b74-106">Integrarea cu Politica de protecție a aplicațiilor Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="86b74-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="86b74-107">Integrarea cu proxy-ul aplicației Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="86b74-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="86b74-108">Comenzi rapide gestionate pentru preferințe și pagini de pornire</span><span class="sxs-lookup"><span data-stu-id="86b74-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="86b74-109">Dacă ați blocat utilizatorii de la înscrierea dispozitivelor mobile, acest scenariu ghidat nu va funcționa, iar utilizatorii vor trebui să instaleze Microsoft Edge pe cont propriu.</span><span class="sxs-lookup"><span data-stu-id="86b74-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="86b74-110">Pentru a implementa Microsoft Edge pentru dispozitive mobile pentru iOS/iPadOS sau Android, consultați:</span><span class="sxs-lookup"><span data-stu-id="86b74-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="86b74-111">Cerințe preliminare</span><span class="sxs-lookup"><span data-stu-id="86b74-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="86b74-112">Introducere</span><span class="sxs-lookup"><span data-stu-id="86b74-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="86b74-113">Bază</span><span class="sxs-lookup"><span data-stu-id="86b74-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="86b74-114">Configurare</span><span class="sxs-lookup"><span data-stu-id="86b74-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="86b74-115">Misiuni</span><span class="sxs-lookup"><span data-stu-id="86b74-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="86b74-116">Revizuire și creare</span><span class="sxs-lookup"><span data-stu-id="86b74-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
