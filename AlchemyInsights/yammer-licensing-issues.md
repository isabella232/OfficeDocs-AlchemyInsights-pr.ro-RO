---
title: Probleme cu licențierea Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657288"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="530e6-102">Probleme cu licențierea Yammer</span><span class="sxs-lookup"><span data-stu-id="530e6-102">Yammer licensing issues</span></span>

<span data-ttu-id="530e6-103">Toți utilizatorii trebuie să aibă o licență pentru a utiliza serviciul Yammer Enterprise, dar în mod implicit Yammer nu necesită ca utilizatorii să aibă o licență pentru a accesa serviciul.</span><span class="sxs-lookup"><span data-stu-id="530e6-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="530e6-104">Atunci când un administrator modifică setarea pentru a bloca utilizatorii Microsoft 365 fără licențe Yammer, utilizatorii cărora nu li s-a atribuit o licență Yammer Enterprise nu pot accesa serviciul Yammer.</span><span class="sxs-lookup"><span data-stu-id="530e6-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="530e6-105">Pentru mai multe informații, consultați [gestionarea licențelor de utilizator Yammer în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="530e6-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="530e6-106">Atunci când licențele sunt eliminate din utilizatori, dala Yammer nu mai este afișată și alte servicii pot utiliza eliminarea licențelor pentru a ascunde caracteristicile.</span><span class="sxs-lookup"><span data-stu-id="530e6-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="530e6-107">În alte cazuri, caracteristicile pot apărea în continuare, dar necesită atribuirea licenței pentru a funcționa.</span><span class="sxs-lookup"><span data-stu-id="530e6-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="530e6-108">**Licența nu se actualizează pentru utilizator**</span><span class="sxs-lookup"><span data-stu-id="530e6-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="530e6-109">Ocazional, unui utilizator i se atribuie o licență, dar încă nu poate accesa Yammer.</span><span class="sxs-lookup"><span data-stu-id="530e6-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="530e6-110">Întârzierile sunt mai susceptibile să apară atunci când este în curs o atribuire a licenței în masă.</span><span class="sxs-lookup"><span data-stu-id="530e6-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="530e6-111">Este posibil ca utilizatorii Yammer să nu fie actualizați în aceeași ordine ca licențele să fie schimbate în Azure AD, deoarece sistemul rulează asincron.</span><span class="sxs-lookup"><span data-stu-id="530e6-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="530e6-112">Așteptați până la 24 de ore înainte de a deschide un caz de asistență pentru a raporta problemele de sincronizare a licențelor.</span><span class="sxs-lookup"><span data-stu-id="530e6-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="530e6-113">**Atribuirea de licențe în masă**</span><span class="sxs-lookup"><span data-stu-id="530e6-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="530e6-114">Licențele pot fi atribuite prin centrul de administrare sau prin scriptarea PowerShell.</span><span class="sxs-lookup"><span data-stu-id="530e6-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="530e6-115">Pentru mai multe informații, consultați [atribuirea de licențe pentru utilizatori](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) și [atribuirea de licențe conturilor de utilizator cu Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="530e6-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="530e6-116">Asistența Microsoft nu oferă asistență pentru crearea de scripturi, dar documentația despre atribuirea licenței Yammer este disponibilă.</span><span class="sxs-lookup"><span data-stu-id="530e6-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="530e6-117">Pentru mai multe informații, consultați [gestionarea licențelor Yammer utilizând Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="530e6-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>