---
title: Problemă cu un singur utilizator
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430204"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="6c10f-102">Problemă cu un singur utilizator</span><span class="sxs-lookup"><span data-stu-id="6c10f-102">Problem with single user</span></span>

- <span data-ttu-id="6c10f-103">Este posibil ca utilizatorul să nu fi fost furnizat, deoarece serviciul nu a avut încă șansa de a evalua utilizatorul.</span><span class="sxs-lookup"><span data-stu-id="6c10f-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="6c10f-104">Revizuiți instrucțiunile pentru durata de furnizare a accesului, precum și bara de progres de pe pagina de configurare a accesului.</span><span class="sxs-lookup"><span data-stu-id="6c10f-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="6c10f-105">Dacă starea de echilibru specificată în secțiunea detalii suplimentare este înainte de data la care utilizatorul a fost creat/actualizat/șters, înseamnă că nu am evaluat încă utilizatorul.</span><span class="sxs-lookup"><span data-stu-id="6c10f-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="6c10f-106">În acest scenariu, cel mai bun lucru de făcut este să așteptați ca serviciul de asigurare a accesului să se termine.</span><span class="sxs-lookup"><span data-stu-id="6c10f-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="6c10f-107">Rețineți că serviciul nostru cunoaște doar modificările aduse unui utilizator din sistemul sursă (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="6c10f-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="6c10f-108">Trebuie să existe o modificare validă în sistemul sursă pentru Azure AD pentru a detecta modificarea și a o debita în Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6c10f-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="6c10f-109">Serviciul de asigurare a accesului a evaluat utilizatorul și a determinat că nu trebuie furnizat:</span><span class="sxs-lookup"><span data-stu-id="6c10f-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="6c10f-110">Dacă ați setat un filtru de definire bazat pe atribut, asigurați-vă că utilizatorul îndeplinește criteriile pe care le-ați specificat.</span><span class="sxs-lookup"><span data-stu-id="6c10f-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="6c10f-111">Dacă utilizatorii există deja în sistemul țintă și în starea utilizatorului în secțiunea sursă și țintă, nu vom mai întreprinde nicio acțiune suplimentară.</span><span class="sxs-lookup"><span data-stu-id="6c10f-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="6c10f-112">Serviciul de asigurare a accesului a încercat să furnizeze utilizatorul și nu a reușit.</span><span class="sxs-lookup"><span data-stu-id="6c10f-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="6c10f-113">Pentru aceste scenarii, examinați fila depanare și recomandări din jurnalele de asigurare a accesului:</span><span class="sxs-lookup"><span data-stu-id="6c10f-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="6c10f-114">Un atribut obligatoriu pentru utilizator poate fi lipsă în Active Directory local sau Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c10f-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="6c10f-115">De exemplu, regulile de generare userPrincipalName sau sAMAccountName nu generează valoarea corectă.</span><span class="sxs-lookup"><span data-stu-id="6c10f-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="6c10f-116">Atributul corespondent (de obicei IDAngajat) nu se rezolvă cu un utilizator unic în Active Directory local sau Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6c10f-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="6c10f-117">De exemplu, există doi utilizatori cu aceeași IDAngajat în AD și serviciul returnează un cod de eroare indicând intrările țintă dublate pentru aceeași intrare sursă.</span><span class="sxs-lookup"><span data-stu-id="6c10f-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="6c10f-118">Pentru a revizui jurnalele pentru un singur utilizator și grupuri, consultați [revizuirea jurnalelor de asigurare a accesului pentru o problemă cu un anumit utilizator](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="6c10f-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
