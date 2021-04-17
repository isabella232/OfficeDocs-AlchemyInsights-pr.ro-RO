---
title: Probleme la conectarea la aplicațiile Microsoft 365
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833087"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="00e24-102">Remedierea aplicațiilor Microsoft 365 Mesaj "Ne pare rău, un alt cont din organizația dvs. este deja conectat"</span><span class="sxs-lookup"><span data-stu-id="00e24-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="00e24-103">Pentru a remedia această eroare, urmați pașii de mai jos:</span><span class="sxs-lookup"><span data-stu-id="00e24-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="00e24-104">Eliminați toate conturile de la locul de muncă, cu excepția contului afectat, utilizând Setări Windows > accesați contul de la locul **de muncă sau de la școală**.</span><span class="sxs-lookup"><span data-stu-id="00e24-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="00e24-105">[Goliți acreditările Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Managerul de acreditări Windows.</span><span class="sxs-lookup"><span data-stu-id="00e24-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="00e24-106">**Notă:** Căile de registry pentru Office 2016 s-au modificat la 16.0.</span><span class="sxs-lookup"><span data-stu-id="00e24-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="00e24-107">(De exemplu: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="00e24-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="00e24-108">Deschideți o aplicație Office, alegeți  >  **Deconectare**  >  **cont de fișier**. Apoi conectați-vă utilizând un cont de utilizator cu o licență validă.</span><span class="sxs-lookup"><span data-stu-id="00e24-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="00e24-109">Pentru informații detaliate, consultați [Conturi din Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="00e24-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="00e24-110">Pentru Mac, consultați [Nu vă puteți conecta la o aplicație Office 2016 pentru Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="00e24-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="00e24-111">Pentru mai multe informații, consultați "Ne pare rău, un alt cont de la organizația [dvs. este deja conectat la acest computer" în Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="00e24-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>