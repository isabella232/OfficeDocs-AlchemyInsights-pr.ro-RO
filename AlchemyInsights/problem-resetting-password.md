---
title: Problemă la reinițializarea parolei
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696275"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="59966-102">Probleme la resetarea parolei</span><span class="sxs-lookup"><span data-stu-id="59966-102">Problems resetting password</span></span>

<span data-ttu-id="59966-103">În continuare, există câteva dintre problemele cu care ați putea face față atunci când reinițializați parola și soluțiile posibile:</span><span class="sxs-lookup"><span data-stu-id="59966-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="59966-104">**Am o problemă cu resetarea parolei care nu este acoperită în celelalte categorii**</span><span class="sxs-lookup"><span data-stu-id="59966-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="59966-105">Asigurați-vă că sunteți autorizat să resetați parole.</span><span class="sxs-lookup"><span data-stu-id="59966-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="59966-106">Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.</span><span class="sxs-lookup"><span data-stu-id="59966-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="59966-107">Administratorii globali pot reseta și alte parole ale administratorului privilegiat.</span><span class="sxs-lookup"><span data-stu-id="59966-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="59966-108">Asigurați-vă că înțelegeți cerințele de licențiere:</span><span class="sxs-lookup"><span data-stu-id="59966-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="59966-109">Trebuie să aveți cel puțin o licență atribuită în organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="59966-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="59966-110">Utilizatori Cloud Only-orice Office 365 (O365) a plătit SKU sau Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="59966-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="59966-111">Utilizatori cloud și/sau locali-Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="59966-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="59966-112">Pentru a citi mai multe despre cerințele de licențiere, consultați articolul [cerințele de licențiere pentru resetarea parolei AZURE AD self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="59966-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="59966-113">**Am probleme la testarea politicii de resetare a parolei setate**</span><span class="sxs-lookup"><span data-stu-id="59966-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="59966-114">Politicile aplicate recent pot dura câteva minute pentru a se reproduce în toate centrele de date și punctele finale.</span><span class="sxs-lookup"><span data-stu-id="59966-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="59966-115">Distanța fizică de la centrul de date va afecta, de asemenea, cât de repede se aplică modificările.</span><span class="sxs-lookup"><span data-stu-id="59966-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="59966-116">Testați cu un utilizator final, nu cu un administrator și pilot cu un set mic de utilizatori.</span><span class="sxs-lookup"><span data-stu-id="59966-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="59966-117">Politicile configurate în portalul Azure se aplică doar pentru utilizatorii finali, nu pentru administratori.</span><span class="sxs-lookup"><span data-stu-id="59966-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="59966-118">Microsoft impune o politică de resetare a parolei cu două porți implicite pentru orice rol de administrator Azure (exemplu: administrator global, administrator Helpdesk, administrator de parole etc.)</span><span class="sxs-lookup"><span data-stu-id="59966-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="59966-119">Aflați mai multe despre [politicile pentru administratori](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="59966-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="59966-120">**Doresc să lansez resetarea parolei, dar nu doresc să fac ca utilizatorii mei să înregistreze informații suplimentare de securitate**</span><span class="sxs-lookup"><span data-stu-id="59966-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="59966-121">Pre-popula date pentru utilizatori, astfel încât aceștia să nu fie nevoiți!</span><span class="sxs-lookup"><span data-stu-id="59966-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="59966-122">-În calitate de administrator, puteți seta proprietățile telefonului și e-mailului pentru utilizatori înainte de a reinițializa parola la organizația dvs.</span><span class="sxs-lookup"><span data-stu-id="59966-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="59966-123">Puteți face acest lucru utilizând un API, PowerShell sau Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="59966-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="59966-124">Mai multe informații aici:</span><span class="sxs-lookup"><span data-stu-id="59966-124">More information here:</span></span>
- [<span data-ttu-id="59966-125">Implementarea resetării parolei fără a solicita utilizatorilor să se înregistreze</span><span class="sxs-lookup"><span data-stu-id="59966-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="59966-126">Ce date se utilizează prin resetarea parolei</span><span class="sxs-lookup"><span data-stu-id="59966-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="59966-127">**Butonul de resetare a parolei este estompat**</span><span class="sxs-lookup"><span data-stu-id="59966-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="59966-128">Nu sunteți autorizat să resetați parolele acestui utilizator.</span><span class="sxs-lookup"><span data-stu-id="59966-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="59966-129">Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.</span><span class="sxs-lookup"><span data-stu-id="59966-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="59966-130">Administratorii globali pot reseta și alte parole ale administratorului privilegiat.</span><span class="sxs-lookup"><span data-stu-id="59966-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="59966-131">**Nu văd lama de resetare a parolei**</span><span class="sxs-lookup"><span data-stu-id="59966-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="59966-132">Nu sunteți autorizat să resetați parole.</span><span class="sxs-lookup"><span data-stu-id="59966-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="59966-133">Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.</span><span class="sxs-lookup"><span data-stu-id="59966-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="59966-134">Administratorii globali pot reseta și alte parole ale administratorului privilegiat.</span><span class="sxs-lookup"><span data-stu-id="59966-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="59966-135">**Nu văd lama de integrare locală în resetarea parolei**</span><span class="sxs-lookup"><span data-stu-id="59966-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="59966-136">Lama de integrare locală apare doar în medii hibride, ceea ce înseamnă că utilizați parole writeback pentru a manipula parolele utilizatorilor locali.</span><span class="sxs-lookup"><span data-stu-id="59966-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="59966-137">Nu vedeți această lamă dacă:</span><span class="sxs-lookup"><span data-stu-id="59966-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="59966-138">Nu utilizați parola writeback</span><span class="sxs-lookup"><span data-stu-id="59966-138">You are not using password writeback</span></span>
    - <span data-ttu-id="59966-139">Există o problemă cu instalarea/conectivitatea parolei writeback</span><span class="sxs-lookup"><span data-stu-id="59966-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="59966-140">Există o problemă cu instalarea/conectivitatea Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="59966-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="59966-141">Pentru mai mulți pași de depanare pentru problemele cu parola writeback, consultați secțiunea [Depanarea parolei writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="59966-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="59966-142">**Nu știu cum să resetez parola unui utilizator**</span><span class="sxs-lookup"><span data-stu-id="59966-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="59966-143">Conectați-vă la portalul Azure ca administrator corespunzător.</span><span class="sxs-lookup"><span data-stu-id="59966-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="59966-144">Accesați lama utilizatori și grupuri, selectați **toți utilizatorii**.</span><span class="sxs-lookup"><span data-stu-id="59966-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="59966-145">Selectați un utilizator din listă.</span><span class="sxs-lookup"><span data-stu-id="59966-145">Select a user from the list.</span></span>
1. <span data-ttu-id="59966-146">Pentru utilizatorul selectat, selectați **Prezentare generală**, apoi, în bara de comenzi, faceți clic pe **Reinițializare parolă**.</span><span class="sxs-lookup"><span data-stu-id="59966-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="59966-147">Urmați instrucțiunile de pe ecran.</span><span class="sxs-lookup"><span data-stu-id="59966-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="59966-148">Se resetează doar prin intermediul parolei de asistență writeback pentru portalul Azure.</span><span class="sxs-lookup"><span data-stu-id="59966-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="59966-149">**Am reinițializat o parolă de utilizator locală din portalul de administrare Office 365 sau din aplicația mobilă Office 365, dar utilizatorul încă nu se poate conecta**</span><span class="sxs-lookup"><span data-stu-id="59966-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="59966-150">Writeback parolelor nu este acceptată în acest portal.</span><span class="sxs-lookup"><span data-stu-id="59966-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="59966-151">Resetarea parolei utilizatorului din nou în portalul Azure-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="59966-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

