---
title: Depanarea problemelor cu înscrierea dispozitivelor Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830954"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="bd4fa-102">Depanarea problemelor cu înscrierea dispozitivelor Android în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bd4fa-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="bd4fa-103">Revizuiți resursele listate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="bd4fa-104">Câțiva pași uzuali pentru probleme și rezolvare:</span><span class="sxs-lookup"><span data-stu-id="bd4fa-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="bd4fa-105">**Eroarea Dispozitiv necriptat din Portalul firmei:** Versiunile mai noi de Android, în special începând cu v7.0, necesită un cod de acces la pornire pentru a vă asigura că dispozitivul dvs. este complet criptat.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="bd4fa-106">Soluțiile obișnuite sunt cele de a activa un cod PIN de pornire sau a cripta complet dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="bd4fa-107">Consultați [acest document pentru](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) mai multe informații.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="bd4fa-108">**Dispozitivele nu reușesc să se verifice cu serviciul Intune sau să se afișeze ca "Nesăcoase" în consola de administrare Intune:** Este posibil ca unele dispozitive Samsung 4.4 și 5.5 să nu intre în serviciu.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="bd4fa-109">Există 3 soluții posibile pentru această problemă:</span><span class="sxs-lookup"><span data-stu-id="bd4fa-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="bd4fa-110">Deschideți manual aplicația Portal firmă Intune, care va iniția automat o sincronizare a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="bd4fa-111">Actualizați dispozitivul la Android 6.0 sau o versiune mai recentă.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="bd4fa-112">Dezactivați Samsung Smart Manager din gestionarea portalului firmei Intune.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="bd4fa-113">Consultați [acest document pentru](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) detalii suplimentare despre aceste probleme și rezolvări.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="bd4fa-114">**Tipul de licență de utilizator** Eroare nevalidă sau Nume de utilizator nerecunoscut: Utilizatorului trebuie să i se atribuie o licență Intune sau EMS. </span><span class="sxs-lookup"><span data-stu-id="bd4fa-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="bd4fa-115">Revizuiți aceste documente pentru a atribui o licență prin: Centrul de administrare Office sau portalul Azure.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="bd4fa-116">Resurse suplimentare care ajută la rezolvarea problemei:</span><span class="sxs-lookup"><span data-stu-id="bd4fa-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="bd4fa-117">Utilizați [Portalul de depanare Intune pentru a diagnostica](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) și a rezolva erorile comune de înscriere.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="bd4fa-118">Consultați [acest document](https://docs.microsoft.com/intune/help-desk-operators) pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="bd4fa-119">Revizuiți [acest document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea și rezolvarea pentru fiecare.</span><span class="sxs-lookup"><span data-stu-id="bd4fa-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="bd4fa-120">[Aflați cum să înscrieți dispozitive Android în Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="bd4fa-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
