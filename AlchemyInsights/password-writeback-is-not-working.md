---
title: Writeback parolelor nu funcționează
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243520"
---
# <a name="password-writeback-is-not-working"></a>Writeback parolelor nu funcționează

**Am probleme cu configurarea parolei writeback**

- Writeback parolelor este o caracteristică premium.
- Asigurați-vă că înțelegeți cerințele de licențiere:
  - Trebuie să aveți cel puțin o licență atribuită în organizația dvs.
  - **Utilizatori Cloud Only** -orice Office 365 (O365) a plătit SKU sau Azure AD Basic
  - **Utilizatori cloud și/sau locali** -Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure productive Enterprise (SPE)
    - Pentru a afla mai multe despre cerințele de licențiere, consultați [cerințe de licențiere pentru resetarea parolei cu autoservire AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Aveți cel puțin un cont de administrator și un cont de utilizator test cu una dintre licențele corespunzătoare.
- Trebuie să conectați Azure AD Connect la emulatorul controlerului de domeniu principal pentru writeback parolei pentru a funcționa. Puteți configura Azure AD Connect pentru a utiliza un controler de domeniu principal, făcând clic dreapta pe **proprietățile** conectorului de sincronizare Active Directory, apoi selectând **configurare partiții directoare**. De acolo, căutați secțiunea **Setări conexiune controler de domeniu** și bifați caseta intitulată **Utilizați doar controlerele de domeniu preferate**.
  > [!NOTE]
  > Dacă DC-ul preferat nu este un emulator PDC, Azure AD Connect va ajunge în continuare la PDC pentru password writeback.
- Resetarea parolei a fost configurată și activată în entitatea găzduită. Pentru mai multe informații, consultați [Activarea utilizatorilor pentru a reseta parolele AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Asigurați-vă că contul de administrator utilizat pentru a activa parola writeback este un cont de administrator Cloud (creat în Azure AD nu AD local)
- Aveți o implementare reclamă locală unică sau mai multe păduri care execută Windows Server 2008 R2, Windows Server 2012 sau Windows Server 2012 R2 cu cele mai recente pachete Service Pack instalate
- Ați instalat instrumentul Azure AD Connect și ați pregătit mediul publicitar pentru sincronizarea cu Cloud. Înainte să testați parola writeback, asigurați-vă că ați finalizat pentru prima dată un import complet și sincronizare completă atât din AD, cât și din Azure AD în Azure AD Connect.
- Pentru a afla mai multe, consultați Cum se face o [Sincronizare completă și importul integral în AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Am o problemă cu conectivitatea writeback prin parolă**

1. Descărcarea și activarea celei mai recente versiuni de [AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configurarea paravanului de protecție: instrumentul Azure AD Connect (1.1.443 și above) va avea nevoie de acces **https de ieșire** la:
    - passwordreset.microsoftonline.com
    - ServiceBus. Windows. Networks
3. Permiteți conexiunilor Idle să persiste cel puțin 2-3 de minute

**Am în continuare probleme cu parola writeback**

- Dacă încă întâmpinați dificultăți, încercați să dezactivați și să activați din nou serviciul de writeback a parolei în instrumentul Azure AD Connect
- Pentru a afla mai multe, consultați Cum să [Dezactivați și să activați din nou parola writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
