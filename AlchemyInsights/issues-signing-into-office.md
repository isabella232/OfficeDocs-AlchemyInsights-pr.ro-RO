---
title: Probleme de sign in la Office apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938310"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="28d97-102">Probleme de sign in la Office apps</span><span class="sxs-lookup"><span data-stu-id="28d97-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="28d97-103">Pentru a remedia problemele de conectare cu Office apps, încercaţi următoarele:</span><span class="sxs-lookup"><span data-stu-id="28d97-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="28d97-104">Elimina toate conturile de muncă, cu excepţia cont afectate, utilizând setări Windows > **acces la munca sau scoala**.</span><span class="sxs-lookup"><span data-stu-id="28d97-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="28d97-105">[Acreditări clar Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizând Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="28d97-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="28d97-106">**Notă:** Căi de registry pentru Office 2016 s-au schimbat la 16,0.</span><span class="sxs-lookup"><span data-stu-id="28d97-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="28d97-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="28d97-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="28d97-108">Deschide o aplicaţie Office, selectaţi **fişier** > **cont** > **Semn afară**. Apoi conectaţi-vă folosind un cont de utilizator cu un permis valabil.</span><span class="sxs-lookup"><span data-stu-id="28d97-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="28d97-109">Pentru informaţii detaliate, consultaţi [conturi în birou](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="28d97-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="28d97-110">Pentru Mac, a se vedea [nu se poate conecta la un Office 2016 pentru Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="28d97-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="28d97-111">În cazul în care erorile apare în timp ce conectarea la Office 365 utilizând Office 2013, permite autentificarea moderne pentru biroul clientului.</span><span class="sxs-lookup"><span data-stu-id="28d97-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="28d97-112">Pentru informații suplimentare, consultați:</span><span class="sxs-lookup"><span data-stu-id="28d97-112">For more information, see:</span></span>
- [<span data-ttu-id="28d97-113">Vă puteţi conecta la Office 365, Azure sau Intune</span><span class="sxs-lookup"><span data-stu-id="28d97-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="28d97-114">Probleme de conectare în semn-înăuntru după update la Office 2016 construi 16.0.7967 pe Windows 10</span><span class="sxs-lookup"><span data-stu-id="28d97-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="28d97-115">"Îmi pare rău, un alt cont la organizaţie este deja autentificat pe acest computer" din Office</span><span class="sxs-lookup"><span data-stu-id="28d97-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="28d97-116">Depanarea sign in probleme cu Office moderne autentificare atunci când utilizaţi perimat</span><span class="sxs-lookup"><span data-stu-id="28d97-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)