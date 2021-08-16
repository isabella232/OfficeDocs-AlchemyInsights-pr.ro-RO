---
title: Depanarea implementării certificatului de autentificare client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020816"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Depanarea implementării certificatului de autentificare client

Profilurile de certificate client Intune NDES/SCEP și PKCS/PFX sunt utilizate de obicei împreună cu alte tipuri de profiluri, cum ar fi Wifi, VPN și e-mailul, pentru a le permite utilizatorilor să se autentifice în resursele corporatiste. Atunci când aceste tipuri de profil sunt legate la un profil de certificat de client depind de implementarea cu succes a profilului respectiv.

Configurarea inițială a infrastructurii și configurarea asociată a profilului certificatului de client necesită adesea depanare. Pentru un ghid pas cu pas pentru configurarea cu succes a conectorului NDES și instrucțiunile de depanare pentru izolarea problemelor cu implementarea certificatelor, consultați: 

- [Configurarea infrastructurii pentru a susține SCEP cu Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Prezentare generală pentru depanarea profilurilor de certificat SCEP cu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Utilizați scripturile PowerShell la care se face referire pentru a verifica configurația. Pentru mai multe informații, consultați [Scripturile de verificare a conectorului Certificat Intune.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Alte probleme comune**

**Atunci când încerc să instalez conectorul de certificat Intune pe serverul de conector NDES, primesc mesajul "Parola din solicitarea de certificat nu poate fi verificată. Este posibil să fi fost utilizat deja. Obțineți o parolă nouă pentru a remite cu această solicitare."**  

Acest mesaj înseamnă că trebuie să rulați instalarea conectorului de certificat ca Administrator.

În unele medii, serverele pe care rulează Certificatul Intune trebuie să utilizeze un server proxy pentru a se conecta la Intune, astfel că Conector certificat trebuie să utilizeze un proxy. În unele circumstanțe, Conectorul NDES ignoră setările proxy configurate și poate fi necesar să configurați setările proxy în timp ce rulează în contextul de securitate din LocalSystem. 
 
Soluția este să rulați Internet Explorer ca SISTEM și să configurați un proxy în IE. După o repornire a Serviciului Conector Intune, NDES Connector se conectează la Intune.

**Dispozitivele de utilizator nu mai primesc certificate SCEP de la NDES.**

Este posibil ca certificatul de autentificare client emis pe serverul NDES și specificat în timpul instalării conectorului NDES să fi expirat sau să lipsească. Pentru a rezolva: 
 
1. Dezinstalați conectorul NDES.  
2. Utilizați aceste detalii pentru a solicita un nou certificat de autentificare client sau autentificare pe server: 
 
    - Nume subiect: CN=fqdn extern  
    - Nume alternativ subiect (ambele sunt necesare): DNS=fqdn extern, DNS=fqdn intern 
 
3. Reinstalați conectorul NDES cu certificatul nou.