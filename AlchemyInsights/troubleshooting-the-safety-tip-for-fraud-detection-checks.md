---
title: Depanarea procesului notificare de siguranță de detectare a fraudelor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955978"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Depanarea procesului notificare de siguranță de detectare a fraudelor

Dacă se afișează un mesaj de e-notificare de siguranță care spune "Expeditorul nu a reușit verificările de detectare a fraudelor și este posibil să nu fie cine pare să fie", expeditorul nu a trecut nici verificările de autentificare DKIM, nici SPF. Cea mai bună metodă de a rezolva această problemă este ca expeditorul să se autorizeze singur. Dacă expeditorul trimite în numele dvs., trebuie să îl autorizați adăugând adresa IP a expeditorului la înregistrarea SPF.
  
Consultați [Depanarea informațiilor roșii (suspecte) notificare de siguranță de detectare a fraudelor pentru](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) mai multe informații.
  
Iată alte câteva linkuri care vă pot ajuta:
  
- [Cum utilizează Microsoft sender Policy Framework (SPF) pentru a preveni falsofingul](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurați SPF pentru a contribui la prevenirea falsării](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
