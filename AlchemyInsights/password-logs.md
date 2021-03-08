---
title: Jurnale de parole
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527179"
---
# <a name="password-logs"></a><span data-ttu-id="dc9f8-102">Jurnale de parole</span><span class="sxs-lookup"><span data-stu-id="dc9f8-102">Password logs</span></span>

<span data-ttu-id="dc9f8-103">**Am probleme cu accesarea jurnalelor de audit de resetare a parolei**</span><span class="sxs-lookup"><span data-stu-id="dc9f8-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="dc9f8-104">Pentru a depana problemele cu privire la accesul la jurnalele de audit de resetare a parolei, efectuați următorul pas:</span><span class="sxs-lookup"><span data-stu-id="dc9f8-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="dc9f8-105">Asigurați-vă că sunteți autorizat să vizualizați jurnalele de auditare.</span><span class="sxs-lookup"><span data-stu-id="dc9f8-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="dc9f8-106">Sunt autorizate doar următoarele roluri:</span><span class="sxs-lookup"><span data-stu-id="dc9f8-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="dc9f8-107">Administrator global</span><span class="sxs-lookup"><span data-stu-id="dc9f8-107">Global administrator</span></span>
 - <span data-ttu-id="dc9f8-108">Administrator de securitate</span><span class="sxs-lookup"><span data-stu-id="dc9f8-108">Security administrator</span></span>
 - <span data-ttu-id="dc9f8-109">Cititor de securitate</span><span class="sxs-lookup"><span data-stu-id="dc9f8-109">Security reader</span></span>

<span data-ttu-id="dc9f8-110">**Doresc să văd toate evenimentele de audit de resetare a parolei din momentul în care am implementat inițial**</span><span class="sxs-lookup"><span data-stu-id="dc9f8-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="dc9f8-111">Până la 120.000 de resetare a parolei/evenimente de înregistrare sunt stocate în rapoartele din ultimele 30 de zile.</span><span class="sxs-lookup"><span data-stu-id="dc9f8-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="dc9f8-112">Această limită maximă se aplică la interfața de utilizator atunci când descărcați CSV.</span><span class="sxs-lookup"><span data-stu-id="dc9f8-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="dc9f8-113">evenimentele 1.000.000 sunt disponibile prin PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dc9f8-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="dc9f8-114">Pentru mai multe informații, consultați linkurile de mai jos:</span><span class="sxs-lookup"><span data-stu-id="dc9f8-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="dc9f8-115">Evenimente de resetare a parolei cu autoservire din API-ul de rapoarte și evenimente Azure AD</span><span class="sxs-lookup"><span data-stu-id="dc9f8-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="dc9f8-116">Cum se descarcă rapid evenimentele de înregistrare a resetării parolelor cu PowerShell</span><span class="sxs-lookup"><span data-stu-id="dc9f8-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="dc9f8-117">**Doresc să înțeleg mai multe despre capacitățile de raportare a resetării parolei**</span><span class="sxs-lookup"><span data-stu-id="dc9f8-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="dc9f8-118">Verificați cine înregistrează sau reinițializează parolele cu jurnalele de audit Azure AD reinițializare a parolelor în portalul Azure, sub **utilizatori și grupuri**.</span><span class="sxs-lookup"><span data-stu-id="dc9f8-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="dc9f8-119">Pentru mai multe informații, consultați următoarele linkuri:</span><span class="sxs-lookup"><span data-stu-id="dc9f8-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="dc9f8-120">Prezentare generală a rapoartelor de resetare a parolei</span><span class="sxs-lookup"><span data-stu-id="dc9f8-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="dc9f8-121">Cum se vizualizează rapoartele de resetare a parolei în portalul Azure</span><span class="sxs-lookup"><span data-stu-id="dc9f8-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="dc9f8-122">Evenimente de resetare a parolei cu autoservire din API-ul de rapoarte și evenimente Azure AD</span><span class="sxs-lookup"><span data-stu-id="dc9f8-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="dc9f8-123">Cum se descarcă rapid evenimentele de înregistrare a resetării parolelor cu PowerShell</span><span class="sxs-lookup"><span data-stu-id="dc9f8-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


