---
title: Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808983"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="8f1d4-102">Depanarea problemelor cu înscrierea dispozitivelor Windows în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8f1d4-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="8f1d4-103">Revizuiți resursele listate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8f1d4-104">Câțiva mesaje de eroare comune și pași de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="8f1d4-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="8f1d4-105">**Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul dvs. de cont a expirat.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="8f1d4-106">Descărcați din nou pachetul de software client pentru PC din consola de administrare Intune.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="8f1d4-107">Consultați această documentație pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="8f1d4-108">**Cod de 0x801c0003:** Eroarea poate apărea în următoarele scenarii:</span><span class="sxs-lookup"><span data-stu-id="8f1d4-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="8f1d4-109">Utilizatorul are mai multe dispozitive înscrise decât limita pentru dispozitive.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8f1d4-110">Revizuiți aceste documente pentru [a elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau a modifica limita pentru [dispozitive.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="8f1d4-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="8f1d4-111">"Utilizatorii pot uni dispozitive la Azure AD" este setată la "fără".</span><span class="sxs-lookup"><span data-stu-id="8f1d4-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="8f1d4-112">Setați-o pentru toți utilizatorii sau selectați-o.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-112">Set it to all or select users.</span></span> <span data-ttu-id="8f1d4-113">Consultați [această documentație](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="8f1d4-114">Dispozitivul este înscris deja de alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="8f1d4-115">În acest caz, eliminați dispozitivul din consola Azure Intune sau anularea manuală a controlului dispozitivului înainte de a încerca din nou.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="8f1d4-116">Dispozitivul este Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="8f1d4-117">Doar SKU-uri Windows 10 Pro, Education și Enterprise se pot alătura Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="8f1d4-118">Resurse suplimentare care ajută la rezolvarea problemei:</span><span class="sxs-lookup"><span data-stu-id="8f1d4-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="8f1d4-119">Utilizați [Portalul de depanare Intune pentru a diagnostica](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) și a rezolva erorile comune de înscriere.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8f1d4-120">Consultați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="8f1d4-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="8f1d4-121">Revizuiți aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvarea pentru [fiecare:](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) Ghid de depanare și [Document de depanare.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="8f1d4-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="8f1d4-122">[Aflați cum să înscrieți dispozitivele Windows în Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="8f1d4-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
