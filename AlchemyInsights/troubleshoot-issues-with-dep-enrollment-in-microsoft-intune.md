---
title: Depanarea problemelor cu înscrierea DEP în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 11b0d73c34996fd84431b38d77b64536d386977e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766721"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="50889-102">Depanarea problemelor cu înscrierea DEP în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="50889-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="50889-103">Examinați resursele enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="50889-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="50889-104">Dacă dispozitivul DEP nu se poate înscrie și ESTE ACTIVATĂ AMF (Autentificare multi-factor), dezactivați MAE.</span><span class="sxs-lookup"><span data-stu-id="50889-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="50889-105">În prezent, AMF nu este acceptată pentru înscrierea DEP</span><span class="sxs-lookup"><span data-stu-id="50889-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="50889-106">Utilizați [Intune Depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva erorile de înscriere comune.</span><span class="sxs-lookup"><span data-stu-id="50889-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="50889-107">Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="50889-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="50889-108">Examinați aceste documente pentru o listă de erori comune care împiedică înscrierea și rezolvările la fiecare: [Ghid de depanare](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) și depanare [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="50889-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="50889-109">[Aflați despre programul de înscriere pe dispozitive](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="50889-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
