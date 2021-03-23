---
title: Sunt blocat de accesul condiționat cu un dispozitiv compatibil
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037074"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Sunt blocat de accesul condiționat cu un dispozitiv compatibil

**Instrumente foarte recomandate**

- [Instrument de depanare a înregistrărilor dispozitivelor](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -un instrument cuprinzător care ajută la depanarea problemelor de înregistrare a dispozitivelor cele mai comune.
- [Test de conectivitate pentru înregistrarea dispozitivului](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -un instrument utilizat pentru a vă asigura că un dispozitiv poate accesa punctele finale ale înregistrării dispozitivelor, sub contul sistemului.
- [Script de curățare a dispozitivului AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -un instrument utilizat pentru a căuta și a gestiona dispozitivele vechi în mediul dvs.

Iată câteva motive comune pentru care este posibil ca accesul condiționat să nu reușească pentru un dispozitiv compatibil sau de ce pot fi primiți utilizatorii dumneavoastră nu puteți **ajunge acolo din mesajul de aici** în timpul unei solicitări de conectare la o resursă organizațională.

1. **Dispozitivul nu se află într-o stare de dispozitiv necesară cu o MDM**:

Validați faptul că dispozitivul este înscris cu un furnizor MDM aprobat, cum ar fi Intune și *marcat ca fiind conform* cu acesta. Pentru mai multe informații despre Intune, consultați acest [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Pentru o mai bună înțelegere a conformității dispozitivelor și a Intune, consultați [utilizarea politicii de conformitate pentru a seta regulile pentru dispozitivele pe care le gestionați cu Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Dacă întâmpinați probleme la înscrierea unui dispozitiv cu Intune, găsiți detaliile de depanare la [Depanarea înscrierii dispozitivelor în Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Pentru asistență suplimentară pentru Intune, creați o solicitare de asistență. Pentru a face acest lucru, vizitați [pagina Ajutor și asistență Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Dispozitivul nu este asociat rețelei de organizații**:

Pentru acces la resurse organizaționale, dispozitivul trebuie să fie conectat la rețeaua organizației, fie prin conexiune directă, fie printr-o rețea virtuală privată (VPN) și, de asemenea, asociată la local sau Azure Active Directory. Pentru a vă asocia la un dispozitiv de lucru la rețeaua organizației, consultați [Asocierea dispozitivului de lucru la rețeaua organizației](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Pentru a înregistra un dispozitiv personal/BYOD, consultați [înregistrarea dispozitivului personal în rețeaua organizației](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Pentru a valida dacă dispozitivul s-a alăturat rețelei, puteți urma pașii pentru dispozitivele înregistrate [aici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) sau [aici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)dispozitivele de lucru. Pentru a domeniul problema la conectivitatea de rețea org, urmați instrucțiunile de mai jos:

    1. Conectați-vă la Windows utilizând contul de la locul de muncă sau de la școală, de exemplu, alain@contoso.com.
    2. Conectați-vă la rețeaua organizației printr-o rețea VPN sau DirectAccess.
    3. După ce sunteți conectat, apăsați **tasta siglă Windows + L** pentru a bloca dispozitivul.
    4. Deblocați dispozitivul utilizând contul de la locul de muncă sau de la școală, apoi încercați din nou să accesați aplicația sau serviciul problematic.

Dacă vedeți din nou mesajul de eroare nu puteți **ajunge acolo** , problema este probabil în altă parte.

3. **Sistemul de operare nu este acceptat**:

Asigurați-vă că sunteți în execuția unei versiuni acceptate a sistemului de operare, inclusiv:

- **Client Windows**: Windows 7 sau o versiune mai recentă

- **Windows Server**: windows Server 2008 R2 sau o versiune mai recentă

- **MacOS**: MacOS X sau o versiune mai recentă

- **Android și iOS**: Cea mai recentă versiune de sisteme de operare pentru dispozitive mobile Android și iOS

4. **Browserul Web nu este acceptat**:

Vă rugăm să găsiți browsere acceptate mai jos. Pentru asistență Chrome cu Windows 1703 sau versiuni mai recente, este necesară o extensie de conturi Windows 10. Pentru Edge 85 +, utilizatorul trebuie să fie conectat pentru a transmite corect informații despre conformitatea dispozitivelor. Pentru mai multe detalii, consultați [aici](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, browser gestionat Intune, Safari
- **Android**: **Microsoft Edge**: browser gestionat Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **MacOS**: Chrome, Safari

Găsiți mai multe informații [despre pașii de](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation) **mai jos pentru mesaje și** depanare.
