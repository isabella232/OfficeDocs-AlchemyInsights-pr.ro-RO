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
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658998"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Depanarea implementării certificatului de autentificare client

Profilurile de certificate client NDES/SCEP și PKCS/PFX sunt utilizate frecvent împreună cu alte tipuri de profiluri, cum ar fi WiFi, VPN și e-mail, pentru a le permite utilizatorilor să se autentifice la resurse corporative. Atunci când acele tipuri de profil sunt legate la un profil de certificat client depind de implementarea cu succes a acelui profil.

Configurarea inițială a infrastructurii și configurarea asociată a profilului de certificat client necesită adesea depanare. Pentru un ghid pas cu pas pentru a configura cu succes conectorul NDES și instrucțiuni de depanare pentru a izola problemele cu implementarea certificatelor, consultați: 

- [Configurarea infrastructurii pentru a accepta SCEP cu Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Prezentare generală pentru depanarea profilurilor de certificat SCEP cu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Utilizați Scripturile PowerShell la care se face referire pentru a vă verifica configurația. Pentru mai multe informații, consultați [scripturi de verificare a conectorului de certificat Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Alte probleme comune**

**Atunci când încerc să instalez conectorul de certificat Intune pe serverul de conector NDES, primesc mesajul "parola din solicitarea de certificat nu poate fi verificată. Este posibil să fi fost utilizat deja. Obțineți o parolă nouă pentru a o trimite cu această solicitare. "**  

Acest mesaj înseamnă că trebuie să ruleze instalarea conectorului de certificat ca administrator.

În unele medii, serverele în care rulează certificatul Intune trebuie să utilizeze un server proxy pentru a se conecta la Intune, astfel încât conectorul de certificat să utilizeze un proxy. În unele împrejurări, conectorul NDES ignoră setările proxy configurate și poate fi necesar să configurați setările proxy în timp ce se execută în contextul de securitate al LocalSystem. 
 
Soluția este să ruleze Internet Explorer ca sistem și să configurați un proxy în IE. După o repornire a serviciului conector Intune, conectorul NDES se conectează la Intune.

**Dispozitivele de utilizator nu mai primesc certificatele SCEP de la NDES.**

Este posibil ca certificatul de autentificare client emis la serverul NDES și specificat în timpul instalării conectorului NDES să fie expirat sau lipsește. Pentru a rezolva: 
 
1. Dezinstalați conectorul NDES.  
2. Utilizați aceste detalii pentru a solicita o nouă autentificare de client sau un certificat de autentificare de server: 
 
    - Nume subiect: CN = FQDN extern  
    - Nume alternativ subiect (ambele sunt necesare): DNS = externe FQDN, DNS = Internal FQDN 
 
3. Reinstalați conectorul NDES cu noul certificat.