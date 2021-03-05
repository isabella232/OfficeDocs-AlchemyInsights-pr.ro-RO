---
title: Problemă cu filtrul atribut și definire
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482919"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="f51af-102">Problemă cu filtrul atribut și definire</span><span class="sxs-lookup"><span data-stu-id="f51af-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="f51af-103">**Problemă cu valorile UPN conflictuale**</span><span class="sxs-lookup"><span data-stu-id="f51af-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="f51af-104">Ziua de lucru pentru ca utilizatorul de publicitate să aibă acces la ziua de lucru pentru asigurarea accesului utilizatorilor de reclame afișează mesajul de eroare **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="f51af-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="f51af-105">Operațiunea nu a reușit, deoarece valoarea UPN furnizată pentru Adăugare/modificare nu este unică la nivel de pădure.</span><span class="sxs-lookup"><span data-stu-id="f51af-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="f51af-106">Detalii despre eroare: **CONSTRAINT_ATT_TYPE-UserPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="f51af-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="f51af-107">Valoarea **UserPrincipalName** pe care un conector de zi de lucru încearcă să o seteze atunci când creați contul de utilizator al reclamei există deja în domeniul de anunțuri țintă.</span><span class="sxs-lookup"><span data-stu-id="f51af-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="f51af-108">Acest lucru implică faptul că, fie (1) utilizatorul există deja, iar verificarea ID-ului de potrivire nu a reușit pentru utilizator sau (2) regula de generare a UPN a generat o valoare conflictuală.</span><span class="sxs-lookup"><span data-stu-id="f51af-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="f51af-109">Iată pașii de rezolvare sugerați:</span><span class="sxs-lookup"><span data-stu-id="f51af-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="f51af-110">Dacă utilizatorul există deja și verificarea ID-ului care se potrivește nu a reușit să conecteze contul zile lucrătoare la contul Active Directory, Verificați dacă atributul ID corespondent (de obicei **IDAngajat**) atât în ziua de lucru, cât și în anunț au o potrivire exactă.</span><span class="sxs-lookup"><span data-stu-id="f51af-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="f51af-111">Dacă nu au o corespondență, este o problemă de date care trebuie remediată.</span><span class="sxs-lookup"><span data-stu-id="f51af-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="f51af-112">De exemplu, dacă IDAngajat din ziua lucrătoare este 001052 și în AD este 1052, atunci motorul de asigurare a accesului nu va reuși să conecteze cele două conturi și va încerca să creeze un utilizator care există deja.</span><span class="sxs-lookup"><span data-stu-id="f51af-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="f51af-113">Soluția în acest caz este să modificați valoarea **IDAngajat** din AD pentru a include zerouri inițiale pentru a-l face 001052.</span><span class="sxs-lookup"><span data-stu-id="f51af-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="f51af-114">Dacă expresia generatoare de UPN nu generează o valoare unică, luați în considerare utilizarea funcției de duplicare **SelectUniqueValue** pentru a genera o valoare unică de fiecare dată.</span><span class="sxs-lookup"><span data-stu-id="f51af-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="f51af-115">**Ziua de lucru pentru asigurarea accesului utilizatorilor AD nu setează valoarea atributului Manager pentru contul de utilizator al RECLAMEi**</span><span class="sxs-lookup"><span data-stu-id="f51af-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="f51af-116">Lucrarea de lucru de ziua de lucru pentru asigurarea accesului utilizatorilor AD nu stabilește valoarea de atribut **Manager** pentru conturile de utilizator de publicitate.</span><span class="sxs-lookup"><span data-stu-id="f51af-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="f51af-117">Există două scenarii posibile atunci când se vede acest comportament:</span><span class="sxs-lookup"><span data-stu-id="f51af-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="f51af-118">Managerul din ziua de lucru nu poate fi rezolvat într-un cont de utilizator de publicitate corespunzător, deoarece managerul nu este în domeniul de aplicare.</span><span class="sxs-lookup"><span data-stu-id="f51af-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="f51af-119">Într-un scenariu **mai multe domenii de publicitate** , managerul din ziua de lucru nu este prezent în același domeniu cu utilizatorul.</span><span class="sxs-lookup"><span data-stu-id="f51af-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="f51af-120">Încercați acești pași pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="f51af-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="f51af-121">Dacă ați definit filtrele de definire, verificați mai întâi dacă managerul este în domeniu și îndeplinește clauza de definire.</span><span class="sxs-lookup"><span data-stu-id="f51af-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="f51af-122">În cazul în care managerul nu îndeplinește filtrul de definire, modificați filtrul, astfel încât managerul să fie, de asemenea, în domeniul operațiunii de asigurare a accesului.</span><span class="sxs-lookup"><span data-stu-id="f51af-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="f51af-123">Dacă aveți mai multe domenii de publicitate, conectorul are o limitare cunoscută a incapacității de a rezolva referințele managerului de domenii.</span><span class="sxs-lookup"><span data-stu-id="f51af-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="f51af-124">Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea accesului automat, consultați [Tutorial: Configurarea zilei de lucru pentru asigurarea accesului automat la utilizatori](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="f51af-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













