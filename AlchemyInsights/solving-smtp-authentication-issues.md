---
title: Activați autentificarea SMTP și depanarea
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077663"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="a5437-102">Activați autentificarea SMTP și depanarea</span><span class="sxs-lookup"><span data-stu-id="a5437-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="a5437-103">Dacă doriți să activați autentificarea SMTP pentru o cutie poștală sau obțineți eroarea "Client ne autentificat", "Autentificarea nu reușește" sau eroarea "SmtpClientAuthentication" cu codul 5.7.57 sau 5.7.3 sau 5.7.139 atunci când încercați să retransmisie e-mail prin autentificarea unui dispozitiv sau a unei aplicații cu Microsoft 365, efectuați aceste trei acțiuni pentru a rezolva problema:</span><span class="sxs-lookup"><span data-stu-id="a5437-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="a5437-104">Dezactivați [setările implicite de securitate Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) comutând **Activați valorile implicite de securitate** la **Nu.**</span><span class="sxs-lookup"><span data-stu-id="a5437-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="a5437-105">a.</span><span class="sxs-lookup"><span data-stu-id="a5437-105">a.</span></span> <span data-ttu-id="a5437-106">Conectați-vă la portalul Azure ca administrator de securitate, administrator de acces condiționat sau administrator global.</span><span class="sxs-lookup"><span data-stu-id="a5437-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="a5437-107">b.</span><span class="sxs-lookup"><span data-stu-id="a5437-107">b.</span></span> <span data-ttu-id="a5437-108">Navigați la Proprietăți Azure Active Directory > **de date**.</span><span class="sxs-lookup"><span data-stu-id="a5437-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="a5437-109">c.</span><span class="sxs-lookup"><span data-stu-id="a5437-109">c.</span></span> <span data-ttu-id="a5437-110">Selectați **Gestionați setările implicite de securitate.**</span><span class="sxs-lookup"><span data-stu-id="a5437-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="a5437-111">d.</span><span class="sxs-lookup"><span data-stu-id="a5437-111">d.</span></span> <span data-ttu-id="a5437-112">Setați **Activați valorile implicite de** securitate **la Nu.**</span><span class="sxs-lookup"><span data-stu-id="a5437-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="a5437-113">e.</span><span class="sxs-lookup"><span data-stu-id="a5437-113">e.</span></span> <span data-ttu-id="a5437-114">Selectați **Salvare**.</span><span class="sxs-lookup"><span data-stu-id="a5437-114">Select **Save**.</span></span>

2. <span data-ttu-id="a5437-115">[Activați remiterea SMTP client](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) pentru cutia poștală licențiată.</span><span class="sxs-lookup"><span data-stu-id="a5437-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="a5437-116">a.</span><span class="sxs-lookup"><span data-stu-id="a5437-116">a.</span></span> <span data-ttu-id="a5437-117">Din caseta Centru de administrare Microsoft 365, accesați **Utilizatori activi** și selectați utilizatorul.</span><span class="sxs-lookup"><span data-stu-id="a5437-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="a5437-118">b.</span><span class="sxs-lookup"><span data-stu-id="a5437-118">b.</span></span> <span data-ttu-id="a5437-119">Accesați fila Mail și, sub Aplicații de e-mail , **selectați** Gestionați **aplicațiile de e-mail**.</span><span class="sxs-lookup"><span data-stu-id="a5437-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="a5437-120">d.</span><span class="sxs-lookup"><span data-stu-id="a5437-120">d.</span></span> <span data-ttu-id="a5437-121">**Asigurați-vă că este bifat SMTP** autentificat (activat).</span><span class="sxs-lookup"><span data-stu-id="a5437-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="a5437-122">e.</span><span class="sxs-lookup"><span data-stu-id="a5437-122">e.</span></span> <span data-ttu-id="a5437-123">Selectați **Salvați modificările.**</span><span class="sxs-lookup"><span data-stu-id="a5437-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="a5437-124">[Dezactivați Multi-Factor Authentication (MFA) pentru](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) cutia poștală licențiată.</span><span class="sxs-lookup"><span data-stu-id="a5437-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="a5437-125">a.</span><span class="sxs-lookup"><span data-stu-id="a5437-125">a.</span></span> <span data-ttu-id="a5437-126">Accesați panoul de Centru de administrare Microsoft 365 și, în meniul de navigare din stânga, **selectați Utilizatori**  >  **utilizatori activi**.</span><span class="sxs-lookup"><span data-stu-id="a5437-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="a5437-127">b.</span><span class="sxs-lookup"><span data-stu-id="a5437-127">b.</span></span> <span data-ttu-id="a5437-128">Selectați **Multi-Factor Authentication.**</span><span class="sxs-lookup"><span data-stu-id="a5437-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="a5437-129">c.</span><span class="sxs-lookup"><span data-stu-id="a5437-129">c.</span></span> <span data-ttu-id="a5437-130">Selectați utilizatorul și **dezactivați Multi-Factor Auth**.</span><span class="sxs-lookup"><span data-stu-id="a5437-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
