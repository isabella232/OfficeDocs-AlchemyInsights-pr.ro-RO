---
title: 401 Eroare neautorizată în SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539944"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Eroare neautorizată în SharePoint

Dacă primiți eroarea "(401) Neautorizat" în SharePoint aceasta poate fi legată de perimarea TLS 1.0/1.1. Pentru mai multe informații, consultați:

- [Pregătirea pentru TLS 1.2 în Office 365 Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Erorile de autentificare apar dacă clientul nu are suport pentru TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Actualizați pentru a activa TLS 1.1 și TLS 1.2 ca protocoale sigure implicite în WinHTTP în Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Dacă utilizatorii sunt în Windows 7, asigurați-vă că verifică suitele [TLS Cipher în Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)