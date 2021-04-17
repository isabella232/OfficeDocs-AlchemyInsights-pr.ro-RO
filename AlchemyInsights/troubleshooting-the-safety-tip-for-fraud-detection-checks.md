---
title: Depanarea sfaturilor de siguranță pentru detectarea fraudelor
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834743"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Depanarea sfaturilor de siguranță pentru detectarea fraudelor

Dacă obțineți un sfat de siguranță care spune "Expeditorul nu a reușit verificările de detectare a fraudelor și este posibil să nu fie cine pare să fie", expeditorul nu a trecut nici verificările de autentificare DKIM, nici SPF. Cea mai bună metodă de a rezolva această problemă este ca expeditorul să se autorizeze singur. Dacă expeditorul trimite în numele dvs., trebuie să îl autorizați adăugând adresa IP a expeditorului la înregistrarea SPF.
  
Consultați [Depanarea sfatului de siguranță roșu (suspect) pentru detectarea fraudelor și a verificărilor](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informații.
  
Iată alte câteva linkuri care vă pot ajuta:
  
- [Cum utilizează Microsoft sender Policy Framework (SPF) pentru a preveni falsofingul](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurați SPF pentru a contribui la prevenirea falsării](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
