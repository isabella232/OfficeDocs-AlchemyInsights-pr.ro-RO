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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014908"
---
# <a name="delete-or-restore-applications"></a>Ștergerea sau restaurarea aplicațiilor

**Pentru a șterge o aplicație din entitatea găzduită AZURE AD**:

1. În **portalul AZURE AD**, selectați **aplicații de întreprindere**. Apoi găsiți și selectați aplicația pe care doriți să o ștergeți.
2. În secțiunea **gestionare** din panoul din stânga, selectați **Proprietăți**.
3. Selectați **Ștergere**, apoi selectați **Da** pentru a confirma că doriți să ștergeți aplicația de la entitatea găzduită Azure AD.

Pentru mai multe informații despre cum să ștergeți o aplicație, consultați [pornire rapidă: ștergerea unei aplicații din entitatea găzduită Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

În PowerShell, cmdletul [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) elimină configurațiile proxy ale aplicației dintr-o anumită aplicație din Azure Active Directory și poate șterge complet aplicația dacă este specificată.

Puteți **restaura o aplicație ștearsă** utilizând PowerShell. După ce aplicația pe care doriți să o restaurați a fost identificată, puteți să o restaurați utilizând [Restaurare-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
