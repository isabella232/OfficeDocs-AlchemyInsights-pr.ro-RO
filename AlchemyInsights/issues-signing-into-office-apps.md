---
title: Probleme de sign in la Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938312"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="38b81-102">Fixarea Office apps "computerului Trusted Platformă module nu funcţionează corect" mesaj</span><span class="sxs-lookup"><span data-stu-id="38b81-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="38b81-103">Pentru a rezolva această eroare, încercaţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="38b81-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="38b81-104">Instalaţi cele mai recente actualizări pentru [Windows](https://support.microsoft.com/help/4027667/windows-10-update) si [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="38b81-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="38b81-105">[Acreditări clar Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="38b81-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="38b81-106">**Notă:** Căi de registry pentru Office 2016 s-au schimbat la 16,0.</span><span class="sxs-lookup"><span data-stu-id="38b81-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="38b81-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="38b81-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="38b81-108">Încercaţi [procesul de recuperare utilizator](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) pentru a rezolva eşecurilor Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="38b81-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="38b81-109">Set EnableADAL = 0 paşii următori:</span><span class="sxs-lookup"><span data-stu-id="38b81-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="38b81-110">Faceţi clic dreapta pe butonul Windows Start, selectaţi **Run**, tastaţi **regedit**şi apoi selectaţi **OK**.</span><span class="sxs-lookup"><span data-stu-id="38b81-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="38b81-111">Selectați **Da** pentru a permite Registry Editor pentru a face modificări la aparatul dvs.</span><span class="sxs-lookup"><span data-stu-id="38b81-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="38b81-112">În Registry Editor, adăugaţi o valoare DWORD **EnableADAL** cu o setare de **0** sub HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="38b81-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="38b81-113">Pentru informaţii suplimentare, consultaţi [probleme de conexiune în semn-înăuntru după update la Office 2016 construi 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="38b81-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>