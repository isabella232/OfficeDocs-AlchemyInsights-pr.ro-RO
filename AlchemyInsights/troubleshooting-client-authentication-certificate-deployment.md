---
title: Depanarea implementării certificatului de autentificare client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555301"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Depanarea implementării certificatului de autentificare client

Intune NDES/SCEP și PKCS/PFX Profilurile de certificate client sunt utilizate în mod obișnuit împreună cu alte tipuri de profiluri, ar fi Wifi, VPN și e-mail pentru a permite utilizatorilor să se autentifice la resursele companiei. Atunci când aceste tipuri de profil sunt legate la un profil de certificat de client depind de implementarea cu succes a acelui profil.

Configurarea inițială a infrastructurii și configurarea asociată a profilului certificatului client necesită adesea depanare. Pentru un ghid pas cu pas pentru configurarea cu succes a conectorului NDES și instrucțiuni de depanare pentru a izola problemele legate de implementarea certificatului, consultați: 

- [Configurarea infrastructurii pentru a accepta SCEP cu Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Prezentare generală pentru depanarea profilurilor de certificate SCEP cu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Utilizați scripturile powershell la care se face referire pentru a vă ajuta să verificați configurația. Pentru mai multe informații, consultați [Scripturile de verificare a conectorilor de certificate Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Alte probleme comune**

**Când încerc să instalez conectorul de certificat Intune pe serverul conector NDES, primesc mesajul, "Parola din solicitarea de certificat nu poate fi verificată. Este posibil să fi fost deja folosit. Obțineți o parolă nouă de trimis cu această solicitare."**  

Acest mesaj înseamnă că trebuie să executați instalarea conectorului de certificat ca administrator.

În unele medii, serverele unde se execută Certificatul Intune trebuie să utilizeze un server proxy pentru a se conecta la Intune, astfel încât Conectorul de certificat trebuie să utilizeze un proxy. În unele circumstanțe, Conectorul NDES ignoră setările proxy configurate și poate fi necesar să configurați setările proxy în timp ce se execută în contextul de securitate al LocalSystem. 
 
Soluția este să executați Internet Explorer ca SISTEM și să configurați un proxy în IE. După repornirea serviciului Intune Connector, conectorul NDES se conectează la Intune.

**Dispozitivele utilizator nu mai primesc certificate SCEP de la NDES.**

Este posibil ca certificatul de autentificare client emis pe serverul NDES și specificat în timpul instalării conectorului NDES, să fi expirat sau să lipsească. Pentru a rezolva: 
 
1. Dezinstalați conectorul NDES.  
2. Utilizați aceste detalii pentru a solicita un nou certificat de autentificare client sau de autentificare server: 
 
    - Nume subiect: CN=fqdn extern  
    - Nume alternativ subiect (ambele sunt necesare): DNS=fqdn extern, DNS=fqdn intern 
 
3. Reinstalați conectorul NDES cu noul certificat.