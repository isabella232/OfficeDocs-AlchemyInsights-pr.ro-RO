---
title: Centrul de administrare Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826391"
---
# <a name="teams-admin-center"></a>Centrul de administrare Teams

Aflați despre gestionarea Teams cu [Centrul de administrare Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Dacă nu reușiți să accesați Centrul de administrare Teams, consultați următoarele:

- Verificați dacă ați permis [Adrese IP Office 365 corespunzătoare și URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) pe fiecare dispozitiv perimetral (firewall etc.) sau în regulile firewall-ului de pe computerul local.
- Verificați dacă informațiile de conectare utilizate pentru a accesa Portalul de administratori Teams corespunde cu numele de utilizator listat în [Portalul de administrare Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Dacă utilizatorii nu apar în Centrul de administrare Teams, consultați următoarele:

- Ați creat utilizatori sau ați atribuit licențe în ultimele 24 de ore? Asigurați-vă că așteptați cel puțin 24 de ore înainte de a deschide un tichet de asistență.
- Verificați dacă ați atribuit licențe corespunzătoare?
- Dacă aveți un Active Directory local, verificați dacă valoarea [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sau adresa SIP din câmpul ProxyAddresses din Active Directory local este unică și formatul se potrivește cu sip: Numele de utilizator al utilizatorului din Centrul de administrare [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Dacă intenționați să mențineți o implementare Skype for Business Server și să aveți utilizatori la domiciliu local și online: urmați "Configurarea hibridă cu Teams și **Skype for Business Online"** din Panoul de control Skype for Business Server și mutați utilizatorii online.
