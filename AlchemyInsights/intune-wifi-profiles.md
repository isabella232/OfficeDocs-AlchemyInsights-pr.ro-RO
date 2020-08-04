---
title: Profiluri Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555318"
---
# <a name="intune-wi-fi-profiles"></a>Profiluri Wi-Fi Intune

Implementarea cu succes a conectivității Wi-Fi pentru clienții MDM depinde de un profil implementat corect, care reflectă cerințele infrastructurii Wi-Fi corporative. Pentru a examina setările corespunzătoare pentru platformele client pe care le investigați, consultați: 

[Adăugarea setărilor Wi-Fi pentru dispozitivele care rulează Android în Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Adăugarea setărilor Wi-Fi pentru dispozitivele dedicate și gestionate de Android Enterprise în Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Adăugarea setărilor Wi-Fi pentru dispozitivele iOS și iPadOS în Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Adăugarea setărilor Wi-Fi pentru Windows 10 și dispozitivele ulterioare în Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Importul setărilor Wi-Fi pentru dispozitivele Windows în Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Probleme comune**

**Implementez un profil Wi-Fi care depinde de un certificat implementat specificat în profilul Wi-Fi. Cu toate acestea, profilurile de configurare afișează o stare de eroare.**

Verificați dacă dispozitivul a primit certificatul.

1. În Intune, accesați **Toate dispozitivele** și selectați dispozitivul > **configurația dispozitivului**.

2. Verificați dacă toate profilurile așteptate sunt listate și într-o stare de succes.

3. Pentru un profil Android, dacă aveți certificate intermediare în lanțul de certificate, asigurați-vă că acestea sunt implementate pe dispozitive Android.

    Pentru a verifica starea certificatului, accesați Profiluri **de configurare dispozitiv**Android intermediar  >  **Profiles**  >  **CA**  >  **Properties**  >  **Trusted Certificate**.

Dacă continuați să vedeți erori, examinați procedurile și secțiunile de depanare. Pentru mai multe informații, consultați [Prezentare generală pentru depanarea profilurilor de certificate SCEP cu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Am implementat un profil Wi-Fi pe un dispozitiv. Intune arată că a avut succes, dar dispozitivul nu se conectează la Wi-Fi.**

O stare reușită înseamnă că Intune a implementat cu succes profilul așa a fost configurat. Cu toate acestea, este posibil ca aceste configurații să nu corespundă cerințelor de rețea și/sau autentificare. Pentru mai multe detalii despre tentativa de conectare, examinați jurnalele din serviciul de infrastructură și autentificare (pe controlerul punctului de acces Wi-Fi și pe serverul NPS/Radius). Poate fi necesar să lucrați cu echipa de infrastructură de rețea sau cu furnizorul terț de Wi-Fi pentru a aduna și a revizui jurnalele.