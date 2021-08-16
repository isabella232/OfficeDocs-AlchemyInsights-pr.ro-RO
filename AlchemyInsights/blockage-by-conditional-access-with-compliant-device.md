---
title: Sunt blocat de Acces condiționat cu dispozitiv conform
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019160"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Sunt blocat de Acces condiționat cu dispozitiv conform

**Instrumentele foarte recomandate**

- [Instrumentul de depanare pentru înregistrarea dispozitivelor](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - un instrument cuprinzător care ajută la depanarea celor mai obișnuite probleme de înregistrare a dispozitivelor.
- [Script de testare a conectivității](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) de înregistrare a dispozitivelor - un instrument utilizat pentru a vă asigura că un dispozitiv poate accesa punctele finale de înregistrare a dispozitivelor de sub contul de sistem.
- [Script de curățare a dispozitivelor Azure AD -](https://github.com/mzmaili/AzureADDeviceCleanup) un instrument utilizat pentru a căuta și a gestiona dispozitivele învechite în mediul dvs.

Iată câteva motive frecvente pentru care accesul condiționat poate să nu  reușescă pentru un dispozitiv compatibil sau motivul pentru care utilizatorii dvs. pot primi un mesaj De aici nu puteți ajunge acolo în timpul unei solicitări de conectare către o resursă organizațională.

1. **Dispozitivul nu se află într-o stare de dispozitiv necesară cu MDM:**

Validați că dispozitivul este înscris cu un furnizor MDM aprobat, cum ar fi Intune, și *marcat drept compatibil.* Pentru mai multe informații despre Intune, consultați acest [document.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Pentru o mai bună înțelegere a conformității dispozitivelor și Intune, consultați Utilizarea politicii de conformitate pentru a seta reguli pentru dispozitivele pe [care le gestionați cu Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Dacă aveți probleme cu înscrierea unui dispozitiv cu Intune, găsiți detalii despre depanare la [Depanarea înscrierii dispozitivelor în Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Pentru asistență Intune suplimentară, creați o solicitare de asistență. Pentru a face acest lucru, [vizitați pagina Ajutor și asistență Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Dispozitivul nu este unit cu rețeaua organizațiilor:**

Pentru a accesa resurse organizaționale, dispozitivul trebuie să fie conectat la rețeaua organizației fie printr-o conexiune directă, fie printr-o rețea virtuală privată (VPN) și să fie conectat la un serviciu local sau Azure Active Directory. Pentru a vă alătura unui dispozitiv de lucru la rețeaua organizației, consultați Asocierea [dispozitivului de lucru la rețeaua organizației.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Pentru a înregistra un dispozitiv personal/BYOD, [consultați Înregistrarea dispozitivului personal în rețeaua organizației.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Pentru a valida dacă dispozitivul s-a conectat la rețea, puteți urma pașii pentru dispozitivele înregistrate aici sau [dispozitivele](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) de lucru [aici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Pentru a domeniul de aplicare a problemei la conectivitatea rețelei organizației, urmați instrucțiunile de mai jos:

    1. Conectați-vă la Windows utilizați contul de la locul de muncă sau de la școală, de exemplu, alain@contoso.com.
    2. Conectare la rețeaua organizației dvs. printr-o rețea VPN sau DirectAccess.
    3. După ce vă conectați, apăsați tasta **siglă Windows+L** pentru a bloca dispozitivul.
    4. Deblocați dispozitivul utilizând contul de la locul de muncă sau de la școală, apoi încercați să accesați din nou aplicația sau serviciul problematic.

Dacă vedeți din nou **mesajul de eroare Nu puteți ajunge acolo de aici,** problema este probabil în altă parte.

3. **Sistemul de operare nu este acceptat:**

Asigurați-vă că rulați o versiune acceptată a sistemului de operare, inclusiv:

- **Windows Client:** Windows 7 sau o versiune mai recentă

- **Windows Server:** Windows Server 2008 R2 sau o versiune mai recentă

- **macOS**: macOS X sau o versiune mai recentă

- **Android și iOS:** Cea mai recentă versiune a sistemelor de operare mobile Android și iOS

4. **Browserul web nu este acceptat:**

Mai jos găsiți browsere acceptate. Pentru asistența Chrome cu Windows 1703 sau versiuni mai recente, este necesară o extensie Windows 10 Conturi de utilizator. Pentru Edge 85+, utilizatorul trebuie să fie conectat corect pentru a transmite corect informațiile despre conformitatea dispozitivului. Pentru mai multe detalii, vedeți [aici](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Browser gestionat Intune, Safari
- **Android**: **Microsoft Edge:** Browser gestionat Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS**: Chrome, Safari

Găsiți mai multe informații **despre mesajul Nu puteți ajunge acolo și** pașii de depanare de [aici](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
