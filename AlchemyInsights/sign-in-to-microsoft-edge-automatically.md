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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398741"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="84d8c-102">Conectarea automată la Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="84d8c-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="84d8c-103">Microsoft Edge utilizează contul implicit al unui sistem de operare pentru a se conecta automat la un utilizator, în funcție de modul în care este configurat dispozitivul utilizatorului.</span><span class="sxs-lookup"><span data-stu-id="84d8c-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="84d8c-104">Scenariile pentru fiecare tip de configurare a dispozitivului și procesul său dependent de conectare al utilizatorului sunt descrise mai jos:</span><span class="sxs-lookup"><span data-stu-id="84d8c-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="84d8c-105">**Dispozitivul este hibrid/AAD-J:** această opțiune este disponibilă în Windows 10, versiunile de nivel inferior windows și versiunile de server corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="84d8c-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="84d8c-106">Utilizatorii sunt conectați automat cu conturile lor Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="84d8c-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="84d8c-107">**Dispozitivul este unit cu domeniul:** această opțiune este disponibilă în Windows 10, în windows de nivel inferior și în versiunile de server corespunzătoare.</span><span class="sxs-lookup"><span data-stu-id="84d8c-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="84d8c-108">În mod implicit, utilizatorii cu conturi de domeniu nu sunt conectați automat; pentru a activa conectarea automată pentru ei, utilizați **politica ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="84d8c-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="84d8c-109">Pentru a activa conectarea automată pentru utilizatorii cu conturi Azure AD, luați în considerare asocierea hibridă la dispozitivele lor.</span><span class="sxs-lookup"><span data-stu-id="84d8c-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="84d8c-110">Contul implicit al sistemului de operare este un cont **Microsoft:** această opțiune este disponibilă în Windows 10 RS3 (versiunea 1709, versiunea 10.0.16299) și versiunile mai recente.</span><span class="sxs-lookup"><span data-stu-id="84d8c-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="84d8c-111">Scenariul este puțin probabil să apară pe dispozitivele de întreprindere.</span><span class="sxs-lookup"><span data-stu-id="84d8c-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="84d8c-112">Cu toate acestea, în cazul în care contul implicit al unui sistem de operare este un cont Microsoft, Microsoft Edge va conecta automat utilizatorul cu contul Microsoft.</span><span class="sxs-lookup"><span data-stu-id="84d8c-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
