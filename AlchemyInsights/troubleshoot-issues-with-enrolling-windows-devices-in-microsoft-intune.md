---
title: Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665844"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="76189-102">Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="76189-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="76189-103">Revizuiți resursele listate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="76189-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="76189-104">Unele mesaje de eroare obișnuite și pașii de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="76189-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="76189-105">**Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul de cont a expirat.</span><span class="sxs-lookup"><span data-stu-id="76189-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="76189-106">Redescărcați pachetul software PC client în consola de administrare Intune.</span><span class="sxs-lookup"><span data-stu-id="76189-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="76189-107">Examinați această documentație pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="76189-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="76189-108">**Cod de eroare 0x801c0003:** Eroarea poate apărea în următoarele scenarii:</span><span class="sxs-lookup"><span data-stu-id="76189-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="76189-109">Utilizatorul are mai multe dispozitive înscrise decât limita de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="76189-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="76189-110">Revizuiți aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau pentru a [modifica limita dispozitivului](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="76189-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="76189-111">"Utilizatorii pot asocia dispozitive la Azure AD" este setată la "none."</span><span class="sxs-lookup"><span data-stu-id="76189-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="76189-112">Setați-l la toate sau selectați utilizatori.</span><span class="sxs-lookup"><span data-stu-id="76189-112">Set it to all or select users.</span></span> <span data-ttu-id="76189-113">Examinați [această documentație](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="76189-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="76189-114">Dispozitivul este deja înscris de un alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="76189-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="76189-115">Dacă acesta este cazul, eliminați dispozitivul din consola Azure Intune sau deînregistrați manual dispozitivul înainte de a încerca din nou.</span><span class="sxs-lookup"><span data-stu-id="76189-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="76189-116">Dispozitivul este Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="76189-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="76189-117">Numai Windows 10 Pro, Education și Enterprise SKUs se pot alătura Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="76189-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="76189-118">Resurse suplimentare pentru a vă rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="76189-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="76189-119">Utilizați [Intune depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva eșecuri de înscriere comune.</span><span class="sxs-lookup"><span data-stu-id="76189-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="76189-120">Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="76189-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="76189-121">Revizuiți aceste documente pentru o listă de erori obișnuite care împiedică înscrierea și rezoluțiile la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) și [Depanare Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="76189-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="76189-122">[Aflați să înregistrați dispozitive Windows în Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="76189-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
