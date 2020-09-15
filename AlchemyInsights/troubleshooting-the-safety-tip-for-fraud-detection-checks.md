---
title: Depanarea Sfatului de siguranță pentru controalele de detectare a fraudei
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658422"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Depanarea Sfatului de siguranță pentru controalele de detectare a fraudei

Dacă primiți un sfat de siguranță care spune "expeditorul nu a reușit să verifice controalele de detectare a fraudei și poate să nu fie cine se pare", atunci expeditorul nu a reușit să treacă de controalele de autentificare DKIM sau SPF. Cea mai bună metodă de a rezolva acest lucru este ca expeditorul să se autorizeze. Dacă expeditorul trimite în numele dvs., trebuie să-i autorizați prin adăugarea adresei IP a expeditorului în înregistrarea SPF.
  
Consultați [Depanarea vârfului de siguranță roșu (suspicios) pentru controalele de detectare a fraudelor](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) pentru mai multe informații.
  
Iată alte câteva linkuri care vă pot ajuta:
  
- [Cum utilizează Microsoft Framework Policy (SPF) pentru a preveni falsificarea](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurați SPF pentru a preveni falsificarea](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
