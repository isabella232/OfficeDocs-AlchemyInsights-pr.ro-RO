---
title: 451 4.7.0 Eroare server temporar. Încercați din nou mai târziu. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812588"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Eroare server temporar. Încercați din nou mai târziu. PRX4

Este posibil să vă confruntați cu o problemă în timp ce trimiteți e-mail prin Smarthost "smtp.office365.com" utilizând metoda de remitere a clientului SMTP și să primiți eroarea: "Eroare server temporar 451 4.7.0. Încercați din nou mai târziu. PRX4 este în cea mai mare parte temporară". 

Asigurați-vă că nu utilizați o cutie poștală partajată pentru remiterea clientului SMTP, deoarece metoda de remitere a clientului SMTP necesită o cutie poștală licențiată pentru a trimite mesaje de e-mail. Totuși, dacă nu utilizați o cutie poștală partajată și problema persistă, verificați următoarele:

1. Activați remiterea SMTP client pentru cutia poștală licențiată utilizată prin rularea acestei comenzi PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    SAU

    1. Accesați fereastra Centru de administrare Microsoft 365 > **Utilizatori activi** și selectați utilizatorul.
    1. Accesați fila Mail din E-> **e-mail >** selectați Gestionați **aplicațiile de e-mail**. 
    1. Asigurați-vă **că este bifată** setarea SMTP autentificată (activată).
    1. Selectați **Salvați modificările.**
    
    Pentru a activa autentificarea SMTP pentru întreaga organizație, rulați această comandă:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Notă:** Din motive de securitate, se recomandă să activați autentificarea SMTP doar pentru cutia poștală utilizată. Setarea la nivel de utilizator suprascrie setarea de la nivelul organizației.

2. Dezactivați setările implicite de securitate Azure, comutând **Activați valorile implicite de securitate** **la Nu:**

    1. Conectați-vă la portalul Azure ca administrator de securitate, administrator de acces condiționat sau administrator global.
    1. Navigați la proprietățile Azure Active Directory >**  și** selectați **Gestionare valori implicite de securitate.**
    1. Setați **comutarea Activați valorile** implicite de securitate la **Nu.**
    1. Selectați **Salvare**.

3. Dezactivați Multi Factor Authentication (MFA) pentru cutia poștală licențiată utilizată.

    1. Accesați panoul de Centru de administrare Microsoft 365 și, în meniul de navigare din stânga, alegeți **Utilizatori**  >  **utilizatori activi**.
    1. Pe pagina **Utilizatori activi,** alegeți **Multi-Factor Authentication**.
    1. Selectați utilizatorul și dezactivați **Multi-Factor Authentication.**

