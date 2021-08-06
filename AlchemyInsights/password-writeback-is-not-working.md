---
title: WriteBackul pentru parole nu funcționează
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
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999756"
---
# <a name="password-writeback-is-not-working"></a>WriteBackul pentru parole nu funcționează

**Am probleme cu configurarea writebackului parolelor**

- Writeback de parole este o caracteristică premium.
- Asigurați-vă că înțelegeți cerințele de licențiere:
  - Trebuie să aveți cel puțin o licență atribuită în organizația dvs.
  - **Doar utilizatorii din** cloud - orice SKU cu plată Office 365 (O365) sau Azure AD Basic
  - **Utilizatori în cloud și/sau** locali - Azure AD Premium P1 sau P2, Enterprise Mobility + Security (EMS) sau Secure Productive Enterprise (SPE)
    - Pentru a afla mai multe despre cerințele de licențiere, consultați [Cerințe de licențiere pentru resetarea parolei cu autoservire Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Aveți cel puțin un cont de administrator și un cont de utilizator de test cu una dintre licențele corespunzătoare.
- Trebuie să conectați azure ad Conectare la emulatorul de controler de domeniu principal pentru ca scrierea parolei să se activez. Puteți configura Azure AD Conectare utilizeze un controler de domeniu principal  făcând clic dreapta pe proprietățile conectorului de sincronizare Active Directory, apoi selectând configurați partițiile **de director.** De acolo, căutați secțiunea **setări conexiune controler domeniu** și bifați caseta intitulată Utilizați doar **controlerele de domeniu preferate.**
  > [!NOTE]
  > Dacă DC-ul preferat nu este un emulator PDC, Azure AD Conectare va contacta în continuare PDC-ul pentru scrierea parolelor.
- Resetarea parolei a fost configurată și activată în entitatea găzduită. Pentru mai multe informații, consultați [Permiterea resetării parolelor Azure AD pentru utilizatori.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Asigurați-vă că acel cont de administrator utilizat pentru a activa WriteBack parola este un cont de administrator în cloud (creat în Azure AD nu în AD local)
- Aveți o implementare locală AD într-o singură pădure sau mai multe care rulează Windows Server 2008 R2, Windows Server 2012 sau Windows Server 2012 R2 cu cele mai recente pachete Service Pack instalate
- Aveți instalat instrumentul de Conectare Azure AD și ați pregătit mediul AD pentru sincronizarea cu mediul cloud. Înainte de a testa scrierea parolelor, asigurați-vă că mai întâi terminați o importare completă și sincronizarea completă din AD și Azure AD în Azure AD Conectare.
- Pentru a afla mai multe, aflați cum să [faceți o sincronizare completă și un import complet în Azure AD Conectare](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Am o problemă cu conectivitatea de writeback a parolelor**

1. Descărcați și activați cea mai [recentă versiune de Azure AD Conectare](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configurarea firewallului: Instrumentul de Conectare Azure AD (1.1.443 și mai nou) va avea nevoie de acces **HTTPS** de ieșire la:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Permiteți ca conexiunile inactive să persiste cel puțin 2-3 minute

**Încă am probleme cu scrierea parolelor**

- Dacă în continuare aveți dificultăți, încercați să dezactivarea și să activați din nou serviciul de writeback al parolei în instrumentul de Conectare Azure AD
- Pentru mai multe informații, aflați cum să [dezactivați și să reactivați scrierea parolelor](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
