---
title: Ștergerea sau restaurarea aplicațiilor
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102583"
---
# <a name="delete-or-restore-applications"></a>Ștergerea sau restaurarea aplicațiilor

**Pentru a șterge o aplicație din entitatea găzduită Azure AD:**

1. În portalul **Azure AD**, selectați **Aplicații enterprise**. Apoi găsiți și selectați aplicația pe care doriți să o ștergeți.
2. În **secțiunea** Gestionare din panoul din stânga, selectați **Proprietăți**.
3. Selectați **Ștergere**, apoi selectați **Da pentru** a confirma că doriți să ștergeți aplicația din entitatea găzduită Azure AD.

Pentru mai multe informații despre cum să ștergeți o aplicație, consultați Pornire rapidă: Ștergerea unei aplicații din entitatea [găzduită Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

În PowerShell, cmdletul [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) elimină configurațiile Proxy aplicație dintr-o anumită aplicație din Azure Active Directory și poate șterge aplicația complet dacă se specifică.

Puteți restaura **o aplicație ștearsă** utilizând PowerShell. După ce a fost identificată aplicația pe care doriți să o restaurați, o puteți restaura utilizând [Restaurare-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
