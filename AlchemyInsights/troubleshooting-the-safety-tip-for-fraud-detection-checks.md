---
title: Depanarea bacșișului de siguranță pentru verificările de detectare a fraudelor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504995"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Depanarea bacșișului de siguranță pentru verificările de detectare a fraudelor

Dacă primiți un sfat de siguranță care spune "Expeditorul nu a reușit verificările noastre de detectare a fraudei și nu poate fi cine par a fi", atunci expeditorul nu a reușit să treacă fie DKIM sau SPF controale de autentificare. Cea mai bună metodă pentru a rezolva acest lucru este pentru expeditor să se autorizeze. Dacă expeditorul trimite în numele dvs., trebuie să-i autorizați adăugând adresa IP a expeditorului la înregistrarea SPF.
  
Consultați [Depanarea vârfului roșu (suspect) de siguranță pentru verificările de detectare a fraudei](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informații.
  
Iată alte câteva link-uri care pot ajuta:
  
- [utilizează Microsoft cadrul de politică expeditor (SPF) pentru a preveni falsificarea](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurarea SPF pentru a preveni falsificarea](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
