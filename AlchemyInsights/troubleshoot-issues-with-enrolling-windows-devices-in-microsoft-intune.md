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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934788"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="757e5-102">Depanarea problemelor cu inscrierea dispozitivele Windows în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="757e5-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="757e5-103">Consultaţi resurse enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="757e5-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="757e5-104">Unele mesaje de eroare comune şi rezoluţie paşi:</span><span class="sxs-lookup"><span data-stu-id="757e5-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="757e5-p101">**Software-ul nu poate fi instalat, 0x80cf4017:** Certificatul dumneavoastră de cont a expirat. Re-Descarca pachetul de programe PC Client în consola de administrare Intune. Revizui această documentaţie pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="757e5-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="757e5-108">**Cod de eroare 0x801c0003:** Eroarea poate apărea în următoarele situaţii:</span><span class="sxs-lookup"><span data-stu-id="757e5-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="757e5-p102">Utilizatorul are mai multe dispozitive înscris decât limita de dispozitiv. Examina aceste documente pentru a [elimina un dispozitiv](https://docs.microsoft.com/intune/devices-wipe) sau [schimba limita de dispozitiv](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="757e5-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="757e5-p103">"Utilizatorii pot adera dispozitive azuriu AD" este setat la "niciunul". Setaţi-l la toate sau selectaţi utilizatorii. Revizui [această documentaţie](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="757e5-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="757e5-p104">Aparatul este înscris de un alt utilizator. Dacă este cazul, eliminaţi dispozitivul din consola de Azure Intune sau unenroll manual aparatul înainte de a încerca din nou.</span><span class="sxs-lookup"><span data-stu-id="757e5-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="757e5-p105">Aparatul este Windows 10 Home. Numai Windows 10 Pro, educaţie şi Enterprise SKU se poate alătura Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="757e5-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="757e5-118">Resurse suplimentare pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="757e5-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="757e5-p106">Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere. Revizuirea [acestui document](https://docs.microsoft.com/intune/help-desk-operators) , pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="757e5-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="757e5-121">Revizuirea acestor documente pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare: [Ghid de depanare](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) şi [Depanare doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="757e5-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="757e5-122">[Aflaţi cum să înscrie dispozitive Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="757e5-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

