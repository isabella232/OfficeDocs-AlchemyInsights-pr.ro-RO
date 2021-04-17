---
title: Probleme la conectarea la aplicațiile Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833016"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="abf4e-102">Remedierea aplicațiilor Microsoft 365 "Modulul Platformă de încredere al computerului nu funcționează corect"</span><span class="sxs-lookup"><span data-stu-id="abf4e-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="abf4e-103">Pentru a remedia această eroare, urmați pașii de mai jos:</span><span class="sxs-lookup"><span data-stu-id="abf4e-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="abf4e-104">Instalați cele mai recente actualizări [pentru Windows](https://support.microsoft.com/help/4027667/windows-10-update) și [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="abf4e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="abf4e-105">[Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.</span><span class="sxs-lookup"><span data-stu-id="abf4e-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="abf4e-106">**Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0.</span><span class="sxs-lookup"><span data-stu-id="abf4e-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="abf4e-107">(De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="abf4e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="abf4e-108">Încercați procesul [de recuperare a utilizatorului pentru](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) a remedia erorile Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="abf4e-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="abf4e-109">Setați EnableADAL = 0 utilizând pașii următori:</span><span class="sxs-lookup"><span data-stu-id="abf4e-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="abf4e-110">Faceți clic dreapta pe butonul Start din Windows, **alegeți Rulare**, **tastați regedit**, apoi alegeți **OK.**</span><span class="sxs-lookup"><span data-stu-id="abf4e-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="abf4e-111">Selectați **Da** pentru a permite editorului de registry să facă modificări la dispozitivul dvs.</span><span class="sxs-lookup"><span data-stu-id="abf4e-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="abf4e-112">În Registry Editor, adăugați o valoare DWORD **de EnableADAL** cu o setare **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="abf4e-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="abf4e-113">Pentru mai multe informații, consultați Probleme de conectare la conectare după actualizarea la [Office 2016, compilarea 16.0.7967 din Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="abf4e-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>