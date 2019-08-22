---
title: PERIMAT Federaţia certificatul expiră
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499903"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="b2fc7-102">PERIMAT Federaţia certificatul expiră</span><span class="sxs-lookup"><span data-stu-id="b2fc7-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="b2fc7-103">Pentru a rezolva această problemă, urmaţi aceşti paşi:</span><span class="sxs-lookup"><span data-stu-id="b2fc7-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="b2fc7-104">Instalaţi Microsoft Azure Active Director modulul pentru Windows PowerShell pe calculator (în cazul în care modulul nu este deja instalat).</span><span class="sxs-lookup"><span data-stu-id="b2fc7-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="b2fc7-105">Pentru aceasta, accesaţi [Manage AD azuriu utilizând Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="b2fc7-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="b2fc7-106">Urmaţi paşii din "scenariul 1: AD FS token-semnarea certificat expirat" secţiunea de [eroare "a fost o problemă de accesarea site-ului" de la AD FS atunci când un utilizator federalizate semnele Office 365, Azure, sau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="b2fc7-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="b2fc7-107">Urmaţi paşii din [Cum pentru a actualiza sau a repara setările de un domeniu federativ în Office 365, Azure, sau Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="b2fc7-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="b2fc7-108">Pentru a afla mai multe despre certificate de Federaţia de reînnoire, a se vedea [Renew Federaţia certificate pentru Office 365 şi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="b2fc7-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
