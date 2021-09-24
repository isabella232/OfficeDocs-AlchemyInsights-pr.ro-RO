---
title: Adăugarea unui subdomn
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506773"
---
# <a name="adding-a-sub-domain"></a>Adăugarea unui subdomn

Subdomiile pot fi adăugate la aceeași entitate găzduită sau la o altă entitate găzduită decât domeniul părinte. În orice caz, trebuie să vă gestionați propriile setări DNS pe site-ul web al registratorului dvs. Dacă ați permis ca Microsoft să vă gestioneze setările DNS cu înregistrări NS sau dacă ați cumpărat domeniul de la Microsoft, nu puteți adăuga subdomenii fără să modificați mai întâi acest lucru.

Adăugați mai întâi domeniul părinte, apoi adăugați subdomerul. Dacă subdomeniul se află în aceeași entitate găzduită, nu este necesară o verificare suplimentară. Dacă adăugați subdomerul la o entitate găzduită separată, înregistrarea Txt DNS este necesară pentru verificarea proprietății înainte de a adăuga domeniul și înregistrările DNS suplimentare pentru serviciile selectate.

- Pentru a adăuga un domeniu sau un subdomeniu, urmați expertul [Adăugare](https://admin.microsoft.com/Adminportal#/Domains/Wizard)domeniu sau adăugați manual domeniul sau subdomeniul,   >  **tasând Setare** domeniu  >  **Adăugare domeniu.**

Dacă este necesar:

- Pentru a modifica cine vă gestionează setările DNS pentru un domeniu existent, accesați **Setări** Domains ,bifați caseta de selectare de lângă domeniu, apoi  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **selectați Manage DNS (Gestionare DNS).** În expert, selectați **Adăugați propriile înregistrări DNS și** finalizați expertul.
- Pentru a adăuga subdomori la un domeniu achiziționat Microsoft, mai întâi transferați domeniul la un alt registrator, apoi efectuați modificarea de mai sus pentru a vă gestiona propriile înregistrări DNS. Pentru instrucțiuni, consultați [Transferarea unui domeniu de la Microsoft la o altă gazdă.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Dacă primiți o eroare care vă spune că domeniul dvs. este deja în uz de către alți membri sau persoane din organizația dvs., va trebui mai întâi să preluați acest cont neprogramat înainte de a utiliza domeniul. Pentru instrucțiuni, consultați [Preluați un director nemaniat ca administrator în Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
