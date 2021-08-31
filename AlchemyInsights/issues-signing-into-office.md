---
title: Probleme la conectarea la Microsoft 365 aplicații
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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744658"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Probleme la conectarea la Aplicații Microsoft 365

Notă: Dacă utilizați o versiune mai veche de Windows (de exemplu, Windows 7 SP1, Windows Server 2008 R2), utilizați remedierea simplă pentru a activa TLS 1.2 în mod implicit. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Pentru mai multe informații, consultați Actualizarea pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)protocoale sigure implicite în WinHTTP în Windows .

Pentru a remedia problemele de conectare cu Microsoft 365, încercați următoarele opțiuni pe computerul afectat:  

- Pentru Windows, consultați [Recomandări despre rezolvarea problemelor comune de conectare](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Pentru Mac, consultați [Nu vă puteți conecta la o aplicație Office 2016 pentru Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Sfat** Pe computerele Windows putem diagnostica și remedia automat pentru dvs. mai multe probleme comune de conectare la Office. Descărcați și rulați **[Asistentul pentru recuperare și asistență pentru Office 365](https://aka.ms/SaRA-OfficeSignInScenario)** pentru a utiliza instrumentul nostru automatizat.

**Notă:** Dezactivarea autentificării moderne (ADAL) sau a managementului conturilor web (WAM) pentru remedierea problemelor de conectare sau de **activare nu este recomandată.** Dacă apar erori în timp ce vă conectați la Microsoft 365 utilizați Office 2013, asigurați-vă că activați autentificarea modernă pentru Office client. [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Pentru acțiuni specifice de depanare, consultați:

[Probleme de conexiune la conectare după actualizarea la Office 2016 compilarea 16.0.7967 pe Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nu vă puteți conecta la contul de organizație, cum ar fi Office 365, Azure sau Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Cum să depanați aplicații non-browser care nu se pot conecta la Office 365, Azure sau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Vi se solicită în mod repetat acreditările din Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)