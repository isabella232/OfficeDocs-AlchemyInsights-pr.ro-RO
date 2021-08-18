---
title: Retransmisia e-mailului prin Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324374"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite mesaje de e-mail

Pentru a afla opțiunile și pașii, consultați [Cum să configurați un dispozitiv multifuncțional sau o aplicație pentru a trimite e-mail utilizând Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Dacă aveți un dispozitiv sau o aplicație care nu mai funcționează recent, cele mai obișnuite probleme sunt:

- **Erori asociate cu autentificarea în timpul utilizării remiterii clientului autentificare SMTP** Am făcut recent câteva modificări legate de modul în care funcționează autentificarea SMTP. Pentru mai multe informații despre cum să rezolvați problemele, consultați secțiunea Nereușită din Remedierea problemelor cu [imprimantele, scanerele](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)și aplicațiile LOB care trimit mesaje de e-mail Microsoft 365 sau Office 365 .
- **Acceptăm doar versiunea TLS 1.2 atunci când facem o conexiune sigură la Office 365** Dacă utilizați Conexiune securizată (TLS), asigurați-vă că dispozitivul dvs. de aplicație acceptă TLS 1.2. Pentru mai multe informații, [consultați Pregătirea pentru TLS 1.2 în Office 365 și Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Pentru alte probleme și soluții, consultați Remedierea problemelor cu [imprimantele, scanerele](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)și aplicațiile LOB care trimit mesaje de e-mail utilizând Microsoft 365 sau Office 365 .

Pentru a vedea dispozitivele afectate, accesați [Raportul clienților cu autentificare SMTP](https://protection.office.com/mailflow/dashboard).

**Notă:** Exchange Online nu se adapta la scenarii de corespondență masivă. Pentru a trimite e-mailuri comerciale în masă (de exemplu, buletine informative pentru clienți), trebuie să utilizați furnizori terți specializați în aceste servicii.
