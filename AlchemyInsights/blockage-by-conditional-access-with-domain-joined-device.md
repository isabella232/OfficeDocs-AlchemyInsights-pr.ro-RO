---
title: Sunt blocat de acces condiționat cu un dispozitiv asociat domeniului
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038100"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Sunt blocat de acces condiționat cu un dispozitiv asociat domeniului

**Instrumente foarte recomandate**

Instrument de depanare a [înregistrărilor dispozitivelor](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -instrumentul care ajută la depanarea problemelor cele mai comune de înregistrare a dispozitivelor.

[Test de conectivitate pentru înregistrarea dispozitivului](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -scriptul care vă ajută să vă asigurați că un dispozitiv poate accesa punctele finale de înregistrare a dispozitivelor de sub contul de sistem.

[Script de curățire a dispozitivului AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -scenariul care vă permite să căutați și să gestionați dispozitivele vechi în mediul dvs.

Iată câteva motive comune pentru care accesul condiționat este posibil să nu reușească un dispozitiv care s-a alăturat unui domeniu (hibrid Azure AD).

1. Nu **există niciun PRT-ul AZURE ad pe dispozitiv** -trebuie să vă asigurați că dispozitivul are simbolul de reîmprospătare primară Azure AD (PRT). Pentru mai multe informații despre PRT, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Pentru a verifica dacă aveți Azure AD PRT, puteți să executați `dsregcmd/status` comanda pe dispozitiv și să verificați dacă "AzureAdPrt" este egal cu "Da".

Dacă "AzureAdPrt" este "nu", verificați următoarele:

- **Indiferent dacă aveți un mediu federativ cu AD FS și este inaccesibil din rețelele de domiciliu ale utilizatorilor**: în acest caz, asigurați-vă că punctele finale "usernamemixed" sunt accesibile de la extranet. Dacă AD FS se află în spatele unei rețele VPN, asigurați-vă că utilizatorii se conectează la VPN și se reconectează la dispozitiv. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Dacă TPM-ul dispozitivului este defect și, prin urmare, nu poate autentifica dispozitivul**: bifați "TPM. msc" pentru a vedea dacă starea TPM este "gata". Dacă nu, rulare `dsregcmd/leave` și permiteți reasocierea dispozitivului la AZURE AD. Apoi încercați din nou. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Utilizați un furnizor de identitate terț, care nu acceptă protocolul WS-Trust**. Așa cum se descrie în documentele noastre, dispozitivele hibrid Azure AD-joint nu pot funcționa în acest caz. Vă rugăm să lucrați cu furnizorul de identitate pentru asistență.

2. **Utilizatorii folosesc browserul Chrome fără ca conturile Windows 10** sau **extensia Office Chrome să utilizeze în mod automat PRT-ul pe dispozitivele pe** care le-ați alăturat sau hibrid-s-a alăturat: aceasta conduce la eșecul oricăror politici de acces condiționat bazate pe dispozitiv, cu mesajul de eroare "dispozitiv neînregistrat" afișat. Pentru a utiliza corect browserul Chrome, trebuie să instalați "conturile Windows 10" sau "extinderea Office la browserul Chrome al utilizatorilor" prin SCCM sau Intune. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Dacă nu este posibil să apăsați extensia de la distanță, notificați-i pe utilizatori să instaleze manual una dintre extensiile de mai sus pentru a accesa aplicațiile din spatele accesului condiționat bazat pe dispozitiv. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Dispozitivul a fost corect AZURE AD Azure s-a alăturat, dar a fost șters sau dezactivat din greșeală, fie din cauza modificărilor de sincronizare din AZURE AD Connect, fie din portalul Azure**: dacă se întâmplă acest lucru, obiectul dispozitiv nu mai este recunoscut ca dispozitiv complet asociat, chiar dacă starea "AzureAdJoined" și "PRT" se afișează ca valid pe dispozitiv.

Pentru a remedia această problemă, rulează `dsregcmd/leave` pe dispozitivele afectate și permiteți-le să se reasocieze la AZURE AD. Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Dacă dispozitivele dumneavoastră sunt în Windows 10, 1809 Update, cu VPN/Cloud proxy și Vedeți problemele cu starea "AzureAdPrt" sau cu orice aplicație cu SSO problemă (Outlook nu se conectează la cutia poștală, chiar dacă ați avut PRT), asigurați-vă că aveți acest patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) sau actualizarea cumulativă din aprilie [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) pentru a împiedica erorile PRT pe acele mașini.

















