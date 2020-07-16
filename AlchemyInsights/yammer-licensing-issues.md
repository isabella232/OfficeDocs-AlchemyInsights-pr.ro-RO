---
title: Probleme de licențiere Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148318"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="e6524-102">Probleme de licențiere Yammer</span><span class="sxs-lookup"><span data-stu-id="e6524-102">Yammer licensing issues</span></span>

<span data-ttu-id="e6524-103">Toți utilizatorii trebuie să aibă o licență pentru a utiliza serviciul Yammer Enterprise, dar în mod implicit Yammer nu solicită ca utilizatorii să aibă o licență pentru a accesa serviciul.</span><span class="sxs-lookup"><span data-stu-id="e6524-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="e6524-104">Când un administrator modifică setarea pentru a bloca utilizatorii Microsoft 365 fără licențe Yammer, utilizatorii cărora nu li se atribuie o licență Yammer Enterprise nu pot accesa serviciul Yammer.</span><span class="sxs-lookup"><span data-stu-id="e6524-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="e6524-105">Pentru mai multe informații, consultați [Gestionarea licențelor de utilizator Yammer în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="e6524-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="e6524-106">Când licențele sunt eliminate de la utilizatori, dala Yammer nu mai este afișată, iar alte servicii pot utiliza eliminarea licenței pentru a ascunde caracteristicile.</span><span class="sxs-lookup"><span data-stu-id="e6524-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="e6524-107">În alte cazuri, caracteristicile pot apărea în continuare, dar necesită atribuirea licenței pentru a funcționa.</span><span class="sxs-lookup"><span data-stu-id="e6524-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="e6524-108">**Licența nu se actualizează pentru utilizator**</span><span class="sxs-lookup"><span data-stu-id="e6524-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="e6524-109">Ocazional, unui utilizator i se atribuie o licență, dar nu poate accesa Yammer.</span><span class="sxs-lookup"><span data-stu-id="e6524-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="e6524-110">Întârzierile sunt mai susceptibile să apară atunci când o atribuire de licență în masă este în curs de desfășurare.</span><span class="sxs-lookup"><span data-stu-id="e6524-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="e6524-111">Este posibil ca utilizatorii Yammer să nu fie actualizați în aceeași ordine în care licențele sunt modificate în Azure AD, deoarece sistemul se execută asincron.</span><span class="sxs-lookup"><span data-stu-id="e6524-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="e6524-112">Așteptați până la 24 de ore înainte de a deschide un caz de asistență pentru a raporta problemele de sincronizare a licenței.</span><span class="sxs-lookup"><span data-stu-id="e6524-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="e6524-113">**Cesiunea licenței în bloc**</span><span class="sxs-lookup"><span data-stu-id="e6524-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="e6524-114">Licențele pot fi atribuite prin intermediul centrului de administrare sau al scripturilor PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e6524-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="e6524-115">Pentru mai multe informații, consultați [Atribuirea licențelor utilizatorilor](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) și [Atribuirea licențelor pentru conturile de utilizator cu Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="e6524-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="e6524-116">Asistența Microsoft nu oferă asistență pentru crearea scripturilor, dar documentația pentru atribuirea licenței Yammer este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="e6524-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="e6524-117">Pentru mai multe informații, consultați [Gestionarea licențelor Yammer utilizând Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="e6524-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>