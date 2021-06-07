---
title: Nu se poate activa Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798692"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="15c1f-102">Nu se poate activa Office</span><span class="sxs-lookup"><span data-stu-id="15c1f-102">Unable to activate Office</span></span>

<span data-ttu-id="15c1f-103">**Notă:** Dacă utilizați o versiune mai veche de Windows (de exemplu, Windows 7), asigurați-vă că TLS 1.2 este activat ca implicit.</span><span class="sxs-lookup"><span data-stu-id="15c1f-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="15c1f-104">Pentru mai multe informații, consultați Actualizare pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)protocoale sigure implicite în WinHTTP în Windows .</span><span class="sxs-lookup"><span data-stu-id="15c1f-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="15c1f-105">Verificați dacă abonamentul dvs. a expirat.</span><span class="sxs-lookup"><span data-stu-id="15c1f-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="15c1f-106">Asigurați-vă că aveți un abonament care permite licențe client, cum ar fi Office 365 Business sau Business Premium, și [ asigurați-vă că utilizatorul are atribuită o licență](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="15c1f-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="15c1f-107">Asigurați-vă că utilizatorul se conectează la Office cu același cont căruia i s-a atribuit licența.</span><span class="sxs-lookup"><span data-stu-id="15c1f-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="15c1f-108">Verificați [pagina de stare a serviciilor Office 365](/office365/enterprise/view-service-health) pentru a vedea dacă există probleme cunoscute cu serviciul.</span><span class="sxs-lookup"><span data-stu-id="15c1f-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="15c1f-109">Verificați firewallul, programul antivirus și setările de proxy pentru a confirma că acestea nu blochează accesul aplicațiilor Microsoft 365 la internet.</span><span class="sxs-lookup"><span data-stu-id="15c1f-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="15c1f-110">Consultați [Adrese URL și intervale de adrese IP Office 365](/office365/enterprise/urls-and-ip-address-ranges "Adrese URL și intervale de adrese IP Office 365").</span><span class="sxs-lookup"><span data-stu-id="15c1f-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="15c1f-111">**Sfat** Pe computerele Windows putem diagnostica și remedia automat pentru dvs. mai multe probleme comune de conectare la Office.</span><span class="sxs-lookup"><span data-stu-id="15c1f-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="15c1f-112">Descărcați și rulați **[Asistentul pentru recuperare și asistență pentru Office 365](https://aka.ms/SaRA-OfficeSignInScenario)** pentru a utiliza instrumentul nostru automatizat.</span><span class="sxs-lookup"><span data-stu-id="15c1f-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="15c1f-113">Utilizați următoarele acțiuni de depanare:</span><span class="sxs-lookup"><span data-stu-id="15c1f-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="15c1f-114">Deschideți o aplicație Office și [deconectați-vă](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) din conturile de utilizator existente.</span><span class="sxs-lookup"><span data-stu-id="15c1f-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="15c1f-115">[Eliminați](/microsoft-365/admin/manage/remove-licenses-from-users) și [reatribuiți](/microsoft-365/admin/manage/assign-licenses-to-users) licența Office, apoi [conectați-vă la Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) utilizând contul de utilizator afectat.</span><span class="sxs-lookup"><span data-stu-id="15c1f-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="15c1f-116">Rulați [Depanatorul de activare](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="15c1f-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="15c1f-117">Resetați starea de activare Office</span><span class="sxs-lookup"><span data-stu-id="15c1f-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Resetați starea de activare Office")
- [<span data-ttu-id="15c1f-118">Efectuarea unei reparări Online a Office</span><span class="sxs-lookup"><span data-stu-id="15c1f-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="15c1f-119">Pentru soluții de depanare suplimentare, consultați:</span><span class="sxs-lookup"><span data-stu-id="15c1f-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="15c1f-120">Erorile de activare și „Produs nelicențiat” în Office</span><span class="sxs-lookup"><span data-stu-id="15c1f-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="15c1f-121">Eroarea „Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu” atunci când activați Office</span><span class="sxs-lookup"><span data-stu-id="15c1f-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)