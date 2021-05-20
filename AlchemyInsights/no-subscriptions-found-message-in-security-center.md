---
title: Nu s-a găsit niciun mesaj de abonament în Centrul de securitate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544120"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="0e150-102">Nu s-a găsit niciun mesaj de abonament în Centrul de securitate</span><span class="sxs-lookup"><span data-stu-id="0e150-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="0e150-103">Dacă în timp ce accesați Centrul de securitate Microsoft Defender obțineți un mesaj "Nu s-au găsit abonamente", înseamnă că Azure Active Directory (AAD) utilizat pentru a conecta utilizatorul la portal nu are o licență Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="0e150-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="0e150-104">Tipul Windows licențele E5 Office E5 sunt licențe separate.</span><span class="sxs-lookup"><span data-stu-id="0e150-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="0e150-105">Deschideți un caz de asistență dacă licența a fost achiziționată, dar nu a fost asigurată pentru această instanță AAD.</span><span class="sxs-lookup"><span data-stu-id="0e150-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="0e150-106">Fie aveți:</span><span class="sxs-lookup"><span data-stu-id="0e150-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="0e150-107">O posibilă problemă de asigurare a accesului pentru licențe.</span><span class="sxs-lookup"><span data-stu-id="0e150-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="0e150-108">Din greșeală, asigurarea accesului la licența către alt Microsoft AAD decât cel utilizat pentru autentificare în serviciu.</span><span class="sxs-lookup"><span data-stu-id="0e150-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>