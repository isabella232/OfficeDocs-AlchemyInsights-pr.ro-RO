---
title: Probleme cu acreditările
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063685"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="a214e-102">Probleme cu acreditările</span><span class="sxs-lookup"><span data-stu-id="a214e-102">Issues with credentials</span></span>

<span data-ttu-id="a214e-103">[Platforma de identitate Microsoft și fluxul de acreditări client 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrie cum să programați direct împotriva fluxului de acordare a acreditărilor client OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="a214e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="a214e-104">**Cum gestionez parola sau acreditările de certificat ale unei aplicații?**</span><span class="sxs-lookup"><span data-stu-id="a214e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="a214e-105">În CLI-ul Azure, puteți să utilizați [acreditarea aplicației de publicitate AZ](https://docs.microsoft.com/cli/azure/ad/app/credential) pentru a șterge, a enumera sau a reinițializa acreditările de certificat sau parola unei aplicații.</span><span class="sxs-lookup"><span data-stu-id="a214e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="a214e-106">**Cum își reinițializează utilizatorii parolele?**</span><span class="sxs-lookup"><span data-stu-id="a214e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="a214e-107">Utilizatorii trebuie să se [înregistreze pentru resetarea parolei cu autoservire](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) înainte să își poată reseta parolele.</span><span class="sxs-lookup"><span data-stu-id="a214e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="a214e-108">După ce un utilizator s-a înregistrat, aceștia pot urmări instrucțiunile din acest articol pentru a-și reseta parola: [resetarea parolei de la locul de muncă sau de la școală](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="a214e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="a214e-109">**Cum își modifică utilizatorii parolele?**</span><span class="sxs-lookup"><span data-stu-id="a214e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="a214e-110">Utilizatorii pot urma pașii din acest articol pentru a-și schimba parolele: [cum să vă modificați parola](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="a214e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="a214e-111">De asemenea, pot [gestiona parole de aplicație pentru verificarea în doi pași](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="a214e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="a214e-112">**Utilizatorul meu primește o eroare la modificarea sau resetarea parolei**</span><span class="sxs-lookup"><span data-stu-id="a214e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="a214e-113">Acest link va furniza informații despre problemele comune care pot apărea atunci când un utilizator încearcă să își reseteze parola: [probleme comune și soluțiile lor](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="a214e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="a214e-114">**Am o problemă la reinițializarea parolei unui utilizator**</span><span class="sxs-lookup"><span data-stu-id="a214e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="a214e-115">Asigurați-vă că sunteți autorizat să resetați parole.</span><span class="sxs-lookup"><span data-stu-id="a214e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="a214e-116">*Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.*</span><span class="sxs-lookup"><span data-stu-id="a214e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="a214e-117">Administratorii globali pot reseta și alte parole ale administratorului privilegiat.</span><span class="sxs-lookup"><span data-stu-id="a214e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="a214e-118">Asigurați-vă că înțelegeți cerințele de licențiere:</span><span class="sxs-lookup"><span data-stu-id="a214e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="a214e-119">Trebuie să aveți cel puțin o licență atribuită în organizația dvs.:</span><span class="sxs-lookup"><span data-stu-id="a214e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="a214e-120">**Utilizatori Cloud Only** -orice Office 365 (O365) a plătit SKU sau Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="a214e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="a214e-121">**Utilizatori cloud și/sau locali** -Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="a214e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="a214e-122">Pentru a afla mai multe despre cerințele de licențiere, consultați [cerințe de licențiere pentru resetarea parolei AZURE AD self-service](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="a214e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="a214e-123">Pentru a reseta parola unui utilizator, găsiți utilizatorul în Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a214e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="a214e-124">Apoi, pe lama generală pentru acel utilizator, faceți clic pe butonul "Reinițializare parolă".</span><span class="sxs-lookup"><span data-stu-id="a214e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="a214e-125">**Butonul de resetare a parolei este estompat**</span><span class="sxs-lookup"><span data-stu-id="a214e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="a214e-126">Nu sunteți autorizat să resetați parolele **acestui** utilizator.</span><span class="sxs-lookup"><span data-stu-id="a214e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="a214e-127">*Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.*</span><span class="sxs-lookup"><span data-stu-id="a214e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="a214e-128">Administratorii globali pot reseta și alte parole ale administratorului privilegiat.</span><span class="sxs-lookup"><span data-stu-id="a214e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="a214e-129">**Nu văd lama de resetare a parolei**</span><span class="sxs-lookup"><span data-stu-id="a214e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="a214e-130">Nu sunteți autorizat să resetați parole.</span><span class="sxs-lookup"><span data-stu-id="a214e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="a214e-131">*Doar administratorii globali, parole și utilizatori pot reseta parole de utilizator.*</span><span class="sxs-lookup"><span data-stu-id="a214e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="a214e-132">Administratorii globali pot reseta și alte parole ale administratorului privilegiat.</span><span class="sxs-lookup"><span data-stu-id="a214e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="a214e-133">**Nu văd lama de integrare locală în resetarea parolei**</span><span class="sxs-lookup"><span data-stu-id="a214e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="a214e-134">Lama de integrare locală apare doar în medii hibride, ceea ce înseamnă că utilizați parole writeback pentru a manipula parolele utilizatorilor locali.</span><span class="sxs-lookup"><span data-stu-id="a214e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="a214e-135">Nu vedeți această lamă dacă:</span><span class="sxs-lookup"><span data-stu-id="a214e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="a214e-136">Nu utilizați parola writeback</span><span class="sxs-lookup"><span data-stu-id="a214e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="a214e-137">Există o problemă cu instalarea/conectivitatea parolei writeback</span><span class="sxs-lookup"><span data-stu-id="a214e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="a214e-138">Există o problemă cu instalarea/conectivitatea Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a214e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="a214e-139">Pentru mai mulți pași de depanare pentru problemele cu parola writeback, consultați [Depanarea parolei writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="a214e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="a214e-140">**Nu știu cum să resetez parola unui utilizator**</span><span class="sxs-lookup"><span data-stu-id="a214e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="a214e-141">Conectați-vă la portalul Azure ca administrator corespunzător.</span><span class="sxs-lookup"><span data-stu-id="a214e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="a214e-142">Accesați lama **utilizatori și grupuri** , selectați **toți utilizatorii**.</span><span class="sxs-lookup"><span data-stu-id="a214e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="a214e-143">Selectați un utilizator din listă.</span><span class="sxs-lookup"><span data-stu-id="a214e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="a214e-144">Pentru utilizatorul selectat, selectați **Prezentare generală**, apoi, în bara de comenzi, selectați **Reinițializare parolă**.</span><span class="sxs-lookup"><span data-stu-id="a214e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="a214e-145">Selectați butonul **Reinițializare parolă** și urmați instrucțiunile de pe ecran.</span><span class="sxs-lookup"><span data-stu-id="a214e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="a214e-146">Se resetează doar prin intermediul parolei de asistență writeback pentru **portalul Azure** .</span><span class="sxs-lookup"><span data-stu-id="a214e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="a214e-147">**Am reinițializat o parolă de utilizator locală din portalul de administrare Office 365 sau din aplicația mobilă Office 365, dar utilizatorul încă nu se poate conecta**</span><span class="sxs-lookup"><span data-stu-id="a214e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="a214e-148">Writeback parolelor nu este acceptată în acest portal.</span><span class="sxs-lookup"><span data-stu-id="a214e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="a214e-149">Reinițializați parola utilizatorului în portalul Azure.</span><span class="sxs-lookup"><span data-stu-id="a214e-149">Reset the user's password again in the Azure portal.</span></span>
