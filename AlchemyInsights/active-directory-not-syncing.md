---
title: Active Directory nu se sincronizează
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930987"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="42e60-102">Active Directory nu se sincronizează</span><span class="sxs-lookup"><span data-stu-id="42e60-102">Active Directory not syncing</span></span>

<span data-ttu-id="42e60-103">Dacă primiți erori de sincronizare, cum ar fi "nicio sincronizare recentă" sau observați starea de sincronizare a directorului în portalul de administrare Office spune "Ultima sincronizare cu mai mult de 3 zile în urmă", cauza poate fi faptul că AADConnect are setări incorecte sau permisiuni insuficiente pentru a efectua o sincronizare.</span><span class="sxs-lookup"><span data-stu-id="42e60-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="42e60-104">Reinstalarea AADConnect utilizând setări expres poate rezolva rapid problema:</span><span class="sxs-lookup"><span data-stu-id="42e60-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="42e60-105">[Descărcați cea mai recentă versiune de AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="42e60-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="42e60-106">[Urmați instrucțiunile pentru instalarea expres.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="42e60-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="42e60-107">Azure AD Connect trebuie să fie instalat pe Windows Server 2012 sau o versiune mai recentă.</span><span class="sxs-lookup"><span data-stu-id="42e60-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="42e60-108">Acest server trebuie să fie asociat la domeniu și poate fi un controler de domeniu sau un server membru.</span><span class="sxs-lookup"><span data-stu-id="42e60-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="42e60-109">Pentru o listă completă a cerințelor de informații Conectare Azure AD și a cerințelor preliminare, consultați Cerințe preliminare pentru [azure ad Conectare.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="42e60-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="42e60-110">Pentru mai multe informații despre conturile de serviciu AADConnect, [consultați Azure AD Conectare: Conturi și permisiuni.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="42e60-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
