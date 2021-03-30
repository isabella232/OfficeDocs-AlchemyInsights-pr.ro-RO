---
title: Depanarea asocierii la Azure AD hibrid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401919"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="68754-102">Depanarea asocierii la Azure AD hibrid</span><span class="sxs-lookup"><span data-stu-id="68754-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="68754-103">Se recomandă ferm să vă asigurați că un dispozitiv poate accesa puncte finale de înregistrare a dispozitivelor din contul de sistem, utilizând [scriptul de testare a conectivității pentru înregistrarea dispozitivelor](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="68754-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="68754-104">În cazul în care configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că revizuiți această[introducere în gestionarea dispozitivelor în Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) pentru a afla cum să controlați dispozitivele cu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68754-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="68754-105">Dacă înregistrați dispozitivele direct în Azure AD și le înscrieți în Intune, asigurați-vă că ați [configurat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) și că aveți [licențierea](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) în locație mai întâi.</span><span class="sxs-lookup"><span data-stu-id="68754-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="68754-106">Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD și AD local.</span><span class="sxs-lookup"><span data-stu-id="68754-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="68754-107">Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="68754-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="68754-108">În plus, în cazul în care configurați înregistrările automate în Active Directory local, va trebui să fiți administrator Active Directory și AD FS (dacă este cazul).</span><span class="sxs-lookup"><span data-stu-id="68754-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="68754-109">Pentru mai multe detalii despre rezolvarea potențialelor probleme cu asocierea hibridă, consultați [Depanarea asocierii hibride](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) pentru configurarea Azure AD asociat și pentru gestionarea dispozitivelor utilizând portalul Azure AD, consultați [Configurarea dispozitivelor Azure AD asociate (asociate cu domenii, local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) și [Gestionarea dispozitivelor utilizând portalul Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="68754-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="68754-110">Pentru a rezolva problemele comune cu asocierea la Azure Active Directory (AD) hibrid, consultați [Întrebări frecvente despre asocierea la Azure AD hibrid](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="68754-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
