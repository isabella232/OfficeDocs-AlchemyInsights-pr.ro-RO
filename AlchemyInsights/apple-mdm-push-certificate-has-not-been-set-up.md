---
title: Certificatul de împingere Apple MDM nu a fost configurat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440013"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Certificatul de împingere Apple MDM nu a fost configurat

Un certificat apple MDM Push Certificate (cunoscut și ca certificat APNS (Apple Push Notification Service) nu a fost configurat pentru abonamentul dvs. Fără un certificat apple MDM push configurat, nu poți să te înscrii și să gestionezi dispozitivele iOS și Mac OS. După ce adăugați certificatul la Intune, utilizatorii pot instala aplicația Portal companie pentru a-și înscrie dispozitivele iOS.

1. Selectați **"Sunt de acord."** pentru a acorda Microsoft permisiunea de a trimite date către Apple.

2. Selectați **Descărcați CSR** solicitarea de semnare a certificatului Intune necesară pentru a crea un certificat de împingere Apple MDM. Fișierul este utilizat pentru a solicita un certificat de relație de încredere de la Portalul de certificate de împingere Apple.

3. Selectează **Creează certificatul de împingere MDM** pentru a accesa portalul apple push certificates. Conectați-vă cu ID-ul Apple al companiei, apoi selectați **Creare certificat**. Selectați **Alegere fișier**, răsfoiți la fișierul de solicitare a semnării certificatului, apoi **selectați Încărcare**. Pe pagina Confirmare, alegeți **Descărcare** pentru a descărca fișierul certificat (.pem) și a salva fișierul local.
 
**Notă:** Certificatul este asociat cu ID-ul Apple utilizat pentru a-l crea. Ca o bună practică, utilizați un ID Apple al companiei pentru activități de gestionare și asigurați-vă că cutia poștală este monitorizată de mai multe persoane sau utilizând o listă de distribuire. Nu folosiți niciodată un ID Apple personal. Folosește același ID Apple pentru a reînnoi Certificatul de împingere Apple la fiecare 12 luni.
 
4. Introduceți ID-ul Apple utilizat pentru a crea certificatul de împingere Apple MDM. Înregistrați acest ID ca memento pentru momentul în care trebuie să reînnoiți certificatul.

5. Accesați fișierul certificat (.pem), alegeți **Deschidere**, apoi alegeți **Încărcare**. Cu certificatul push, Intune se poate înscrie și gestiona dispozitivele Apple.