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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049356"
---
# <a name="teams-admin-center"></a>Centrul de administrare Teams

Aflați despre gestionarea Teams cu [Centrul de administrare Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Dacă nu reușiți să accesați Centrul de administrare Teams, consultați următoarele:

- Verificați dacă ați permis [Adrese IP Office 365 corespunzătoare și URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) pe fiecare dispozitiv perimetral (firewall etc.) sau în regulile firewall-ului de pe computerul local.
- Verificați dacă informațiile de conectare utilizate pentru a accesa Portalul de administratori Teams corespunde cu numele de utilizator listat în [Portalul de administrare Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Dacă utilizatorii nu apar în Centrul de administrare Teams, consultați următoarele:

- Ați creat utilizatori sau ați atribuit licențe în ultimele 24 de ore? Asigurați-vă că așteptați cel puțin 24 de ore înainte de a deschide un tichet de asistență.
- Verificați dacă ați atribuit licențe corespunzătoare?
- Dacă aveți un Active Directory local, verificați dacă valoarea [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sau adresa SIP din câmpul ProxyAddresses din Active Directory local este unică și formatul se potrivește cu sip: Numele de utilizator al utilizatorului din [Centru de administrare Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Dacă intenționați să păstrați o implementare Skype for Business Server și să aveți utilizatori acasă la sediul local și online: urmați "Configurarea hibridă cu Teams și **Skype for Business Online"** din Panoul de control Skype for Business Server și mutați utilizatorii online.
