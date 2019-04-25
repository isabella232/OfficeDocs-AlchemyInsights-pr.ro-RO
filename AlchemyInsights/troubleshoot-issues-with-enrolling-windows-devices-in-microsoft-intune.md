---
title: Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390655"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="488ce-102">Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="488ce-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="488ce-103">Consultaţi resurse enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="488ce-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="488ce-104">Unele mesaje de eroare comune şi rezoluţie paşi:</span><span class="sxs-lookup"><span data-stu-id="488ce-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="488ce-105">**Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul dumneavoastră de cont a expirat.</span><span class="sxs-lookup"><span data-stu-id="488ce-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="488ce-106">Re-Descarca pachetul de programe PC Client în consola de administrare Intune.</span><span class="sxs-lookup"><span data-stu-id="488ce-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="488ce-107">Revizui această documentaţie pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="488ce-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="488ce-108">**Cod de eroare 0x801c0003:** Eroarea poate apărea în următoarele situaţii:</span><span class="sxs-lookup"><span data-stu-id="488ce-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="488ce-109">Utilizatorul are mai multe dispozitive înscris decât limita de dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="488ce-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="488ce-110">Examina aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau [schimba limita de dispozitiv](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="488ce-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="488ce-111">"Utilizatorii pot adera dispozitive azuriu AD" este setat la "niciunul".</span><span class="sxs-lookup"><span data-stu-id="488ce-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="488ce-112">Setaţi-l la toate sau selectaţi utilizatorii.</span><span class="sxs-lookup"><span data-stu-id="488ce-112">Set it to all or select users.</span></span> <span data-ttu-id="488ce-113">Revizui [această documentaţie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="488ce-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="488ce-114">Aparatul este înscris de un alt utilizator.</span><span class="sxs-lookup"><span data-stu-id="488ce-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="488ce-115">Dacă este cazul, eliminaţi dispozitivul din consola de Azure Intune sau unenroll manual aparatul înainte de a încerca din nou.</span><span class="sxs-lookup"><span data-stu-id="488ce-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="488ce-116">Aparatul este Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="488ce-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="488ce-117">Numai Windows 10 Pro, educaţie şi Enterprise SKU se poate alătura Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="488ce-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="488ce-118">Resurse suplimentare pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="488ce-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="488ce-119">Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere.</span><span class="sxs-lookup"><span data-stu-id="488ce-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="488ce-120">Revizuirea [acestui document](https://docs.microsoft.com/intune/help-desk-operators) , pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="488ce-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="488ce-121">Revizuirea acestor documente pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare: [Ghid de depanare](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) şi [Depanare doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="488ce-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="488ce-122">[Aflaţi cum să înscrie dispozitive Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="488ce-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

