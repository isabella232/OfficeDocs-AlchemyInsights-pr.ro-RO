---
title: Certificatul de federalizare ADFS expiră
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710419"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="d601a-102">Certificatul de federalizare ADFS expiră</span><span class="sxs-lookup"><span data-stu-id="d601a-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="d601a-103">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="d601a-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="d601a-104">Instalați Microsoft Azure Active Directory Module pentru Windows PowerShell pe computer (dacă modulul nu este deja instalat).</span><span class="sxs-lookup"><span data-stu-id="d601a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="d601a-105">Pentru aceasta, accesați [Gestionarea Azure AD utilizând Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="d601a-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="d601a-106">Urmați pașii din secțiunea "Scenariul 1: Certificatul de semnare a simbolului AD FS a expirat" din ["A existat o problemă la accesarea site-ului" eroare din AD FS atunci când un utilizator federativ se conectează la Microsoft 365, Azure sau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="d601a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="d601a-107">Urmați pașii din [Actualizarea sau repararea setărilor unui domeniu federativ în Microsoft, Azure sau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="d601a-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="d601a-108">Pentru a afla mai multe despre reînnoirea certificatelor de federalizare, consultați [Reînnoirea certificatelor de federalizare pentru Microsoft 365 și Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="d601a-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
