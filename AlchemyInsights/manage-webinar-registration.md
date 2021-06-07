---
title: Gestionarea înregistrării webinar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793910"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="b53bd-102">Gestionarea înregistrării webinar</span><span class="sxs-lookup"><span data-stu-id="b53bd-102">Manage webinar registration</span></span>

<span data-ttu-id="b53bd-103">Puteți gestiona persoanele care se pot înregistra pentru Teams webinars, utilizând Teams powershell.</span><span class="sxs-lookup"><span data-stu-id="b53bd-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="b53bd-104">Pentru a Teams Powershell, consultați [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="b53bd-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="b53bd-105">În mod implicit, *WhoCanRegister* este activat și setat la **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="b53bd-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="b53bd-106">Pentru a permite înregistrării tuturor utilizatorilor anonimi, trebuie să setați politica de întâlnire **la Oricine,** utilizând comanda Powershell:</span><span class="sxs-lookup"><span data-stu-id="b53bd-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="b53bd-107">**Notă:** dacă asocierea anonimă este dezactivată în setările întâlnirii, utilizatorii anonimi nu se pot alătura la webinarii.</span><span class="sxs-lookup"><span data-stu-id="b53bd-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="b53bd-108">Pentru a afla mai multe și a activa această setare, [consultați Gestionarea setărilor întâlnirii din Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="b53bd-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="b53bd-109">Dacă doriți să dezactivați înregistrarea întâlnirilor, *setați AllowMeetingRegistration* la **False**.</span><span class="sxs-lookup"><span data-stu-id="b53bd-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="b53bd-110">Pentru a afla mai multe despre configurarea cine se poate înregistra pentru webinarii, consultați [Configurarea cine se poate înregistra pentru webinarii.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="b53bd-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="b53bd-111">Pentru mai multe informații despre setările pentru Liste Microsoft, consultați [Controlați setările pentru Liste Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="b53bd-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
