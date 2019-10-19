---
title: Certificat de federalizare ADFS expirând
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
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737201"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="aa825-102">Certificat de federalizare ADFS expirând</span><span class="sxs-lookup"><span data-stu-id="aa825-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="aa825-103">Pentru a rezolva această problemă, urmați acești pași:</span><span class="sxs-lookup"><span data-stu-id="aa825-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="aa825-104">Instalați Microsoft Azure Active Directory Module pentru Windows PowerShell pe computer (dacă modulul nu este deja instalat).</span><span class="sxs-lookup"><span data-stu-id="aa825-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="aa825-105">Pentru aceasta, du-te pentru a [gestiona AZURE AD utilizând Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="aa825-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="aa825-106">Urmați pașii din "scenariul 1: AD FS token-semnarea certificatului expirat" secțiunea ["nu a fost o problemă accesarea site-ului" eroare la AD FS atunci când un utilizator federalizate semne în Office 365, Azure sau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="aa825-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="aa825-107">Urmați pașii din [actualizarea sau repararea setărilor unui domeniu federalizate în Office 365, Azure sau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="aa825-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="aa825-108">Pentru a afla mai multe despre reînnoirea certificatelor de federalizare, consultați [reînnoirea certificatelor de federalizare pentru Office 365 și Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="aa825-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
