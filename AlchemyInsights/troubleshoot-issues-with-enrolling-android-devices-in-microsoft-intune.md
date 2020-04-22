---
title: Depanarea problemelor legate de înscrierea dispozitivelor Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759632"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ccecf-102">Depanarea problemelor legate de înscrierea dispozitivelor Android în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ccecf-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ccecf-103">Examinați resursele enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="ccecf-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ccecf-104">Unele probleme comune și etape de rezolvare:</span><span class="sxs-lookup"><span data-stu-id="ccecf-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ccecf-105">**Dispozitiv nu criptate eroare în companie Portal:** Versiunile mai noi de Android, în special începând cu v7.0, necesită un cod de acces la pornire pentru a vă asigura că dispozitivul este complet criptat.</span><span class="sxs-lookup"><span data-stu-id="ccecf-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ccecf-106">Soluțiile comune sunt pentru a activa un pin de pornire sau pentru a cripta complet dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="ccecf-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ccecf-107">Examinați [acest document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pentru mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="ccecf-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ccecf-108">**Dispozitivele nu reușesc să se consulte cu serviciul Intune sau afișați ca "Nesănătoase" în consola de administrare Intune:** Este posibil ca unele dispozitive Samsung 4.4 și 5.5 să nu se verifice în serviciu.</span><span class="sxs-lookup"><span data-stu-id="ccecf-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ccecf-109">Există 3 soluții posibile la această problemă:</span><span class="sxs-lookup"><span data-stu-id="ccecf-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ccecf-110">Deschideți manual aplicația Intune Company Portal, care va iniția automat o sincronizare a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="ccecf-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ccecf-111">Actualizați dispozitivul la Android 6.0 sau mai recent.</span><span class="sxs-lookup"><span data-stu-id="ccecf-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ccecf-112">Dezactivați Samsung Smart Manager de la gestionarea Portalului companiei Intune.</span><span class="sxs-lookup"><span data-stu-id="ccecf-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ccecf-113">Revizuiți [acest document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pentru detalii suplimentare cu privire la aceste probleme și rezolvări.</span><span class="sxs-lookup"><span data-stu-id="ccecf-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ccecf-114">**Tip de licență utilizator Invalid** sau **Nume utilizator Nerecunoscut eroare:** Utilizatorului trebuie să i se atribuie o licență Intune sau EMS.</span><span class="sxs-lookup"><span data-stu-id="ccecf-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ccecf-115">Examinați aceste documente pentru a atribui o licență prin: Office Admin Center sau portalazure.</span><span class="sxs-lookup"><span data-stu-id="ccecf-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ccecf-116">Resurse suplimentare pentru a ajuta la rezolvarea problemei:</span><span class="sxs-lookup"><span data-stu-id="ccecf-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ccecf-117">Utilizați [Intune Depanare portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica și rezolva erorile de înscriere comune.</span><span class="sxs-lookup"><span data-stu-id="ccecf-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ccecf-118">Examinați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="ccecf-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ccecf-119">Examinați [acest document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea și rezolvările pentru fiecare.</span><span class="sxs-lookup"><span data-stu-id="ccecf-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ccecf-120">[Aflați să înscrieți dispozitive Android în Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ccecf-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
