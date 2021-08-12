---
title: Activați autentificarea SMTP și depanarea
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
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957220"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Activați autentificarea SMTP și depanarea

Dacă doriți să activați autentificarea SMTP pentru o cutie poștală sau obțineți eroarea "Client ne autentificat", "Autentificarea nu reușește" sau eroarea "SmtpClientAuthentication" cu codul 5.7.57 sau 5.7.3 sau 5.7.139 atunci când încercați să retransmisie e-mail prin autentificarea unui dispozitiv sau a unei aplicații cu Microsoft 365, efectuați aceste trei acțiuni pentru a rezolva problema:

1. Dezactivați [setările implicite de securitate Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) comutând **Activați valorile implicite de securitate** la **Nu.**

    a. Conectați-vă la portalul Azure ca administrator de securitate, administrator de acces condiționat sau administrator global.<BR/>
    b. Navigați la Proprietăți Azure Active Directory > **de date**.<BR/>
    c. Selectați **Gestionați setările implicite de securitate.**<BR/>
    d. Setați **Activați valorile implicite de** securitate **la Nu.**<BR/>
    e. Selectați **Salvare**.

2. [Activați remiterea SMTP client](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) pentru cutia poștală licențiată.

    a. Din caseta Centru de administrare Microsoft 365, accesați **Utilizatori activi** și selectați utilizatorul.<BR/>
    b. Accesați fila Mail și, sub Aplicații de e-mail , **selectați** Gestionați **aplicațiile de e-mail**.<BR/>
    d. **Asigurați-vă că este bifat SMTP** autentificat (activat).<BR/>
    e. Selectați **Salvați modificările.**<BR/>

3. [Dezactivați Multi-Factor Authentication (MFA) pentru](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) cutia poștală licențiată.

    a. Accesați panoul de Centru de administrare Microsoft 365 și, în meniul de navigare din stânga, **selectați Utilizatori**  >  **utilizatori activi**.<BR/>
    b. Selectați **Multi-Factor Authentication.**<BR/>
    c. Selectați utilizatorul și **dezactivați Multi-Factor Auth**.<BR/>
