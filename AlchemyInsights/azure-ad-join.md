---
title: Asociere Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405675"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="a8daa-102">Asociere Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a8daa-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="a8daa-103">În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit Introducere în gestionarea dispozitivelor în [Azure Active Directory,](/azure/active-directory/devices/overview) care vă va ghida cum să duceți dispozitivele sub controlul Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a8daa-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="a8daa-104">Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, va trebui să [](/mem/intune/fundamentals/licenses-assign) vă asigurați că ați configurat [Intune](/mem/intune/enrollment/device-enrollment) și că licențierea a fost configurată mai întâi.</span><span class="sxs-lookup"><span data-stu-id="a8daa-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="a8daa-105">Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a8daa-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="a8daa-106">Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="a8daa-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="a8daa-107">Pentru a face implementarea uniării Azure AD, consultați [Planificarea Azure AD Join.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="a8daa-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="a8daa-108">Pentru mai multe detalii despre rezolvarea problemelor comune cu Azure AD Join, consultați Întrebări frecvente despre [Azure Ad Join](/azure/active-directory/devices/faq) și pentru dispozitivul Windows 10 pro, consultați Nu puteți să vă asociați computerului Windows 10 Pro la Azure AD - Trebuie să faceți upgrade la [- Comunitatea Microsoft.](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="a8daa-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
