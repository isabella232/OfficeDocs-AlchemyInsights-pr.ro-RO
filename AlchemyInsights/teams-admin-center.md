---
title: Centrul de administrare Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670376"
---
# <a name="teams-admin-center"></a>Centrul de administrare Teams

Aflați despre gestionarea Teams cu [Centrul de administrare Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Dacă nu reușiți să accesați Centrul de administrare Teams, consultați următoarele:

- Verificați dacă ați permis [Adrese IP Office 365 corespunzătoare și URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) pe fiecare dispozitiv perimetral (firewall etc.) sau în regulile firewall-ului de pe computerul local.
- Verificați dacă informațiile de conectare utilizate pentru a accesa Portalul de administratori Teams corespunde cu numele de utilizator listat în [Portalul de administrare Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Dacă utilizatorii nu apar în Centrul de administrare Teams, consultați următoarele:

- Ați creat utilizatori sau ați atribuit licențe în ultimele 24 de ore? Asigurați-vă că așteptați cel puțin 24 de ore înainte de a deschide un tichet de asistență.
- Verificați dacă ați atribuit licențe corespunzătoare?
- Dacă aveți un Director activ local, Verificați dacă [Valoarea msRTCSIP-PrimaryUserAddress sau adresa SIP din câmpul ProxyAddresses din directorul active locale este unică și formatul se potrivește cu](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**numele de utilizator** al utilizatorului din [Centrul de administrare Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Dacă intenționați să păstrați o implementare Skype for Business Server și să aveți utilizatori conectați local și online: urmați opțiunea **"configurați hibridul cu teams și Skype for Business Online"** din panoul de control Skype for Business Server și mutați utilizatorii online.
