---
title: Conectarea automată la Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678813"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="a5ff7-102">Conectarea automată la Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a5ff7-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="a5ff7-103">Microsoft Edge utilizează contul implicit al sistemului de operare pentru a se conecta automat la un utilizator în funcție de modul în care este configurat dispozitivul utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="a5ff7-104">Scenariile pentru fiecare tip de configurație a dispozitivului și procesul de conectare la utilizatorul său dependent sunt descrise mai jos:</span><span class="sxs-lookup"><span data-stu-id="a5ff7-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="a5ff7-105">**Dispozitivul este hibrid/AAD-J**: această opțiune este disponibilă în Windows 10, Windows level și versiunile de server corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="a5ff7-106">Utilizatorii sunt conectați automat cu conturile lor Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="a5ff7-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="a5ff7-107">**Dispozitivul este asociat domeniului**: această opțiune este disponibilă în Windows 10, Windows level și versiunile de server corespondente.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="a5ff7-108">În mod implicit, utilizatorii cu conturi de domeniu nu sunt conectați automat; pentru a activa conectarea automată pentru ele, utilizați Politica **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="a5ff7-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="a5ff7-109">Pentru a activa conectarea automată pentru utilizatori cu conturi de publicitate Azure, luați în considerare conectarea hibridă a dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="a5ff7-110">**Contul implicit al sistemului de operare este un cont Microsoft**: această opțiune este disponibilă în Windows 10 RS3 (versiunea 1709, compilarea 10.0.16299) și versiunile ulterioare.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="a5ff7-111">Scenariul este puțin probabil să apară pe dispozitivele Enterprise.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="a5ff7-112">Cu toate acestea, dacă contul implicit al sistemului de operare este un cont Microsoft, atunci Microsoft Edge se va conecta automat la utilizator cu contul Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5ff7-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
