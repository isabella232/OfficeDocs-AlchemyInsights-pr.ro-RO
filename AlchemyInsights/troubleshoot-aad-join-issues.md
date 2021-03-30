---
title: Depanarea problemelor de asociere Azure AD
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405758"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="b5d60-102">Depanarea problemelor de asociere Azure AD</span><span class="sxs-lookup"><span data-stu-id="b5d60-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="b5d60-103">În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit Introducere în gestionarea dispozitivelor în [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) care vă va ghida cum să duceți dispozitivele sub controlul Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b5d60-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="b5d60-104">Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, va trebui să [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) vă asigurați că ați configurat [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) și că licențierea a fost configurată mai întâi.</span><span class="sxs-lookup"><span data-stu-id="b5d60-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="b5d60-105">Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b5d60-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="b5d60-106">Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="b5d60-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="b5d60-107">Pentru a face implementarea uniării Azure AD, consultați [Planificarea Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="b5d60-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="b5d60-108">Pentru mai multe detalii despre rezolvarea problemelor comune cu Azure AD join consultați Întrebări frecvente despre [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) și pentru dispozitivul Windows 10 pro, consultați Nu se poate alătura computerului [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) la Azure AD - Trebuie să faceți upgrade la - Comunitatea Microsoft</span><span class="sxs-lookup"><span data-stu-id="b5d60-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
