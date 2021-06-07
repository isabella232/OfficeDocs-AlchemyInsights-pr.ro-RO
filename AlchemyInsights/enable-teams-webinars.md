---
title: Activarea Teams webinarii
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793781"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="d96b7-102">Activarea Teams webinarii</span><span class="sxs-lookup"><span data-stu-id="d96b7-102">Enable Teams Webinars</span></span>

<span data-ttu-id="d96b7-103">Webinariile sunt activate implicit.</span><span class="sxs-lookup"><span data-stu-id="d96b7-103">Webinars are enabled by default.</span></span> <span data-ttu-id="d96b7-104">Puteți gestiona cine poate programa și înregistra pentru Teams webinars, utilizând Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d96b7-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="d96b7-105">Toți utilizatorii care pot crea o întâlnire pot crea, de asemenea, o întâlnire webinar.</span><span class="sxs-lookup"><span data-stu-id="d96b7-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="d96b7-106">Dacă doriți să gestionați cine poate programa Teams webinarii, *utilizați AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="d96b7-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="d96b7-107">În mod implicit, *WhoCanRegister* este activat și setat la **Oricine.**</span><span class="sxs-lookup"><span data-stu-id="d96b7-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="d96b7-108">Dacă doriți să dezactivați înregistrarea întâlnirilor, *setați AllowMeetingRegistration* la **False**.</span><span class="sxs-lookup"><span data-stu-id="d96b7-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="d96b7-109">Pentru a modifica aceste setări, trebuie să [instalați Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="d96b7-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="d96b7-110">De asemenea, politicile de întâlnire sunt impuse Teams webinarii.</span><span class="sxs-lookup"><span data-stu-id="d96b7-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="d96b7-111">De exemplu, dacă asocierea anonimă este dezactivată în setările întâlnirii, utilizatorii anonimi nu se pot alătura la webinarii.</span><span class="sxs-lookup"><span data-stu-id="d96b7-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="d96b7-112">Pentru a afla mai multe despre configurarea cine se poate înregistra pentru webinarii, consultați [Configurarea cine se poate înregistra pentru webinarii.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="d96b7-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="d96b7-113">Pentru mai multe informații despre setările pentru Liste Microsoft, consultați [Controlați setările pentru Liste Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="d96b7-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>