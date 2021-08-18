---
title: Remedierea problemelor uzuale cu Microsoft Defender pentru Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330072"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Remedierea problemelor uzuale cu Microsoft Defender pentru Office 365

Iată câteva soluții la problemele obișnuite cu Microsoft Defender pentru Office 365:

- **Întârziere mesaj:**

  Întârzierile în livrarea mesajelor de e-mail pot fi cauzate Seif de scanarea atașărilor de mesaje. Pentru mai multe informații, [consultați Seif de politică pentru Atașări.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Raportarea rezultatelor fals pozitive sau negative:**

  Pentru mai multe informații, consultați [Raportarea mesajelor și fișierelor la Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Activarea Seif protecție împotriva legăturilor:**

  1. În portalul Microsoft 365 Defender la , accesați Trimitere prin <https://security.microsoft.com/> **e-mail &** Politicilor de colaborare & Reguli Seif Linkuri către linkuri \>  \>  \>  **din secțiunea** Politici.

     Pentru a merge direct la **Seif Linkuri** rapide, utilizați <https://security.microsoft.com/safelinksv2> .

  2. Pe pagina **Seif Linkuri,** selectați politica, făcând clic pe numele politicii.
  3. În fișa cu detalii care apare, urmați oricare dintre pașii următori:
     - Pentru a adăuga o politică nouă, selectați **+ Creare**. Se va lansa un expert care vă va ajuta să definiți setările de politică.
     - Pentru a edita o politică existentă, selectați politica, făcând clic pe numele politicii. În meniul volant detalii care apare, selectați **Editare** în **secțiunea Setări protecție.**
  4. Pe pagina **Setări protecție,** configurați următoarele setări:
     - Activare **Selectați acțiunea pentru ADRESE URL potențial rău intenționate necunoscute din mesaje.**
     - Selectați **Aplicați linkuri sigure la mesajele trimise în cadrul organizației.**

  Pentru mai multe informații, [consultați Configurarea Seif privind linkurile din Microsoft Defender pentru Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
