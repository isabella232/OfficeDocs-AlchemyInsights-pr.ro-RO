---
title: Implementarea Microsoft Edge la iOS, iPadOS și Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194590"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="c41f4-102">Implementarea Microsoft Edge la iOS, iPadOS și Android</span><span class="sxs-lookup"><span data-stu-id="c41f4-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="c41f4-103">Scenariul ghidat rezumat mai jos vă va ajuta să atribuiți Microsoft Edge utilizatorilor de dispozitive iOS, iPadOS și Android.</span><span class="sxs-lookup"><span data-stu-id="c41f4-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="c41f4-104">Dacă ați blocat utilizatorii de la înscrierea dispozitivelor mobile, acest scenariu ghidat nu va funcționa, iar utilizatorii vor trebui să instaleze Microsoft Edge singuri.</span><span class="sxs-lookup"><span data-stu-id="c41f4-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="c41f4-105">Scenariul ghidat implică următorii pași:</span><span class="sxs-lookup"><span data-stu-id="c41f4-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="c41f4-106">Cerințe preliminare</span><span class="sxs-lookup"><span data-stu-id="c41f4-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="c41f4-107">Introducere</span><span class="sxs-lookup"><span data-stu-id="c41f4-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="c41f4-108">Bază</span><span class="sxs-lookup"><span data-stu-id="c41f4-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="c41f4-109">Configurare</span><span class="sxs-lookup"><span data-stu-id="c41f4-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="c41f4-110">Misiuni</span><span class="sxs-lookup"><span data-stu-id="c41f4-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="c41f4-111">Revizuire și creare</span><span class="sxs-lookup"><span data-stu-id="c41f4-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="c41f4-112">După ce terminați pașii din scenariul ghidat, politicile Microsoft Intune vor activa următoarele caracteristici Microsoft Edge pentru Business:</span><span class="sxs-lookup"><span data-stu-id="c41f4-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="c41f4-113">Identitate dublă</span><span class="sxs-lookup"><span data-stu-id="c41f4-113">Dual identity</span></span>
- <span data-ttu-id="c41f4-114">Integrarea cu Politica de protecție a aplicațiilor Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c41f4-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="c41f4-115">Integrarea cu proxy-ul aplicației Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c41f4-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="c41f4-116">Comenzi rapide gestionate pentru preferințe și pagini de pornire</span><span class="sxs-lookup"><span data-stu-id="c41f4-116">Managed favorites and home page shortcuts</span></span>
