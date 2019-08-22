---
title: Depanarea problemelor cu inscrierea dispozitive Android în Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500083"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="58538-102">Depanarea problemelor cu inscrierea dispozitive Android în Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="58538-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="58538-103">Consultaţi resurse enumerate mai jos pentru a rezolva problema acum.</span><span class="sxs-lookup"><span data-stu-id="58538-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="58538-104">Unele probleme comune şi rezoluţie paşi:</span><span class="sxs-lookup"><span data-stu-id="58538-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="58538-105">**Aparat nu criptate eroare în compania Portal:** Versiunile mai noi de Android, în special începând cu v7.0, cere o parola de startup pentru a vă asigura că dispozitivul este complet criptat.</span><span class="sxs-lookup"><span data-stu-id="58538-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="58538-106">Soluţiile comune sunt pentru a activa un cod pin startup sau cripta complet dispozitivul.</span><span class="sxs-lookup"><span data-stu-id="58538-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="58538-107">Revizuirea [acestui document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , pentru mai multe informaţii.</span><span class="sxs-lookup"><span data-stu-id="58538-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="58538-108">**Dispozitive nu verifica cu serviciul Intune sau afişa ca "Nesanatoase" în consola de administrare Intune:** Unele 4.4 Samsung şi 5,5 dispozitive pot verifica în service.</span><span class="sxs-lookup"><span data-stu-id="58538-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="58538-109">Există 3 posibile soluţii la această problemă:</span><span class="sxs-lookup"><span data-stu-id="58538-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="58538-110">Manual deschide aplicaţia Portal de compania Intune, care va iniţia automat o sincronizare dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="58538-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="58538-111">Actualizați dispozitivul Android 6.0 sau mai mare.</span><span class="sxs-lookup"><span data-stu-id="58538-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="58538-112">Dezactivaţi Samsung Smart Manager la gestionarea Intune compania Portal.</span><span class="sxs-lookup"><span data-stu-id="58538-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="58538-113">Revizuirea [acestui document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , pentru mai multe detalii despre aceste probleme şi rezoluţii.</span><span class="sxs-lookup"><span data-stu-id="58538-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="58538-114">**User a da un permis tip nevalid** sau **User nume nu a fost recunoscut eroarea:** utilizatorul trebuie să li se atribuie o licenţă Intune sau EMS.</span><span class="sxs-lookup"><span data-stu-id="58538-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="58538-115">Examina aceste documente pentru a atribui o licenţă prin: centrul de administrare Office sau Azure portal.</span><span class="sxs-lookup"><span data-stu-id="58538-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="58538-116">Resurse suplimentare pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="58538-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="58538-117">Utilizaţi [Intune depanare Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) pentru a diagnostica şi rezolva comune eşecuri de înscriere.</span><span class="sxs-lookup"><span data-stu-id="58538-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="58538-118">Revizuirea [acestui document](https://docs.microsoft.com/intune/help-desk-operators) , pentru mai multe detalii.</span><span class="sxs-lookup"><span data-stu-id="58538-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="58538-119">Consultaţi [acest document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pentru o listă de erori comune care împiedică înscrierea şi rezoluţii pentru fiecare.</span><span class="sxs-lookup"><span data-stu-id="58538-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="58538-120">[Aflaţi cum să înscrie dispozitive Android în Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="58538-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
