---
title: Programul de completare teams pentru Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629827"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="cb2d3-102">Programul de completare teams pentru Mac</span><span class="sxs-lookup"><span data-stu-id="cb2d3-102">Teams add-in for Mac</span></span>

<span data-ttu-id="cb2d3-103">Pentru a depana un program de completare teams care lipsește pentru utilizatorii sistemului de operare Mac, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="cb2d3-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="cb2d3-104">**Pasul 1:** Dacă aveți Exchange hibrid local (2016 CU3 sau o versiune mai recentă), utilizați instrumentul de Test-HMA.ps1 pentru a confirma că autentificarea modernă hibridă este configurată corect.</span><span class="sxs-lookup"><span data-stu-id="cb2d3-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="cb2d3-105">Pentru mai multe informații, consultați [validarea instalării hibride moderne de autentificare pentru Outlook pentru iOS și Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="cb2d3-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="cb2d3-106">**Notă** Utilizați formatul de adresă UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)), nu domain\username.</span><span class="sxs-lookup"><span data-stu-id="cb2d3-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="cb2d3-107">Faceți acest lucru chiar și pentru utilizatorii cu cutii poștale Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="cb2d3-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="cb2d3-108">**Pasul 2:** Să aibă utilizatorul Accesați conturile de **Instrumente**  >  **Accounts**... în Outlook pentru Mac și găsiți și selectați contul.</span><span class="sxs-lookup"><span data-stu-id="cb2d3-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="cb2d3-109">Confirmați numele de utilizator listat este în format UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="cb2d3-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="cb2d3-110">**Pasul 3:** Confirmați că utilizatorul este un utilizator Microsoft teams licențiat.</span><span class="sxs-lookup"><span data-stu-id="cb2d3-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="cb2d3-111">Utilizatorul trebuie să utilizeze abonamentul Office 365 pentru Mac, versiunea de produs 16,24 sau o versiune mai recentă.</span><span class="sxs-lookup"><span data-stu-id="cb2d3-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>