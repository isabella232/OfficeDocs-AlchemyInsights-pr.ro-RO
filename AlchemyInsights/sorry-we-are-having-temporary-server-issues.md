---
title: Remedierea Microsoft 365 Aplicații personale Ne pare rău, avem mesaje de probleme temporare despre server
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
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744679"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Remedierea problemelor Microsoft 365 mesajele "Ne pare rău, avem probleme temporare pe server"

Notă: Dacă utilizați o versiune mai veche de Windows (de exemplu, Windows 7 SP1, Windows Server 2008 R2), utilizați remedierea simplă pentru a activa TLS 1.2 în mod implicit. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Pentru mai multe informații, consultați Actualizarea pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)protocoale sigure implicite în WinHTTP în Windows .

Dacă primiți acest mesaj, încercați următoarele:

1. Verificați firewallul, software-ul antivirus și setările proxy pentru a confirma că nu blochează accesul la internet la Microsoft 365 aplicații. Consultați [URL-uri și intervale de adrese IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Accesați **Start**  >  **Run**, apoi tastați **services.msc**. Asigurați-vă că toate serviciile următoare rulează:
    - Configurarea automată a dispozitivelor conectate la rețea
    - Serviciul Listă de rețea
    - Informații despre locația de rețea
    - Windows Jurnalul de evenimente

Dacă unul dintre aceste servicii nu rulează, încercați să îl porniți. Dacă aveți o problemă la pornirea serviciului, rulați următoarea comandă deschizând o linie de comandă cu permisiuni cu drepturi înălțimii:

**sfc /scannow**

După ce se termină această comandă, reporniți computerul.

Pentru informații detaliate, [consultați "Ne pare rău, nu ne putem conecta la contul dvs. Încercați din nou mai târziu" atunci când activați.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)