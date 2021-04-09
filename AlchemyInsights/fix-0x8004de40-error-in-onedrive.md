---
title: Remedierea 0x8004de40 eroare în OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649760"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Remedierea 0x8004de40 eroare în OneDrive

Dacă rulați Windows 7 și primiți această eroare, Actualizați pentru a activa [TLS 1.1 și TLS 1.2 ca](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)protocoale sigure implicite în WinHTTP în Windows .

Dacă rulați Windows 10 și primiți o eroare 0x8004de40 cu OneDrive:

- Reporniți computerul afectat în timp ce sunteți conectat la domeniul Acitve Directory.
- Dacă o repornire nu remediază problema, anulați-vă și reasezați-vă dispozitivul din Azure AD. 

**Notă:** Ar trebui să vă a afla în rețeaua de corporație în timp ce efectuați acești pași. Nu efectuați acești pași atunci când nu sunteți conectat la infrastructura de corporație (de exemplu, în timpul călătoriilor). 

1. Deschideți o linie de comandă cu drepturi înălțimii selectând **Start,** faceți clic **dreapta pe Linie de** comandă, apoi **selectați Rulare ca administrator**.

1. Tastați *dsregcmd /leave și* apăsați **pe Enter**.

1. Când terminați, tastați *dsregcmd /join și* apăsați pe **Enter**.

1. Când terminați, închideți linia de comandă.

1. Reporniți computerul și conectați-vă la OneDrive.