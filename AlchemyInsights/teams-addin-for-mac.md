---
title: Teams de completare pentru Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582082"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="e6fad-102">Teams de completare pentru Mac</span><span class="sxs-lookup"><span data-stu-id="e6fad-102">Teams add-in for Mac</span></span>

<span data-ttu-id="e6fad-103">Pentru a depana un Teams de completare pentru utilizatorii sistemului de operare Mac, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="e6fad-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="e6fad-104">**Pasul 1:** Dacă aveți autentificare hibridă Exchange (2016 CU3 sau o versiune mai recentă), utilizați instrumentul Test-HMA.ps1 pentru a confirma că autentificarea modernă hibridă este configurată corect.</span><span class="sxs-lookup"><span data-stu-id="e6fad-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="e6fad-105">Pentru mai multe informații, [consultați Validarea configurării de autentificare modernă hibridă pentru Outlook pentru iOS și Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="e6fad-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="e6fad-106">**Notă** Utilizați formatul DE ADRESĂ UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)), nu domeniul \numeutilizator.</span><span class="sxs-lookup"><span data-stu-id="e6fad-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="e6fad-107">Faceți acest lucru chiar și pentru utilizatorii Exchange Online poștale.</span><span class="sxs-lookup"><span data-stu-id="e6fad-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="e6fad-108">**Pasul 2:** Spuneți utilizatorului să meargă **la Conturi**  >  **instrumente...** în Outlook pentru Mac și găsiți și selectați contul.</span><span class="sxs-lookup"><span data-stu-id="e6fad-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="e6fad-109">Confirmați că numele de utilizator listat este în format UPN (de exemplu, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="e6fad-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="e6fad-110">**Pasul 3:** Confirmați că utilizatorul este utilizator cu Microsoft Teams licențe.</span><span class="sxs-lookup"><span data-stu-id="e6fad-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="e6fad-111">Utilizatorul trebuie să folosească abonamentul Office 365 Mac, versiunea de produs 16.24 sau o versiune mai recentă.</span><span class="sxs-lookup"><span data-stu-id="e6fad-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>