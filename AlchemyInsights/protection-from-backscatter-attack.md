---
title: Protecție împotriva atacului prin puncte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037176"
---
# <a name="protection-from-backscatter-attack"></a>Protecție împotriva atacului prin puncte

Mesajele de completare sunt rapoarte de nelivrare (denumite și mesaje rapoarte NDR sau sarituri) pe care le primiți pentru mesajele pe care nu le-ați trimis. Spammeri Forge (spoof) de **la:** adresa mesajelor lor și folosesc deseori adrese de e-mail reale pentru a-și acorda credibilitate mesajelor. Așadar, atunci când autorii de spam trimit în mod inevitabil mesaje către destinatari inexistenți, serverul de e-mail de destinație este în esență păcălit să returneze mesajul nelivrat într-un NDR către expeditorul falsificat în adresa **de la:** .

Informații suplimentare pot fi găsite în [puncte de completare în EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Activarea protecției prin puncte**

Pentru a activa protecția prin puncte, urmați calea de mai jos.

**protection.office.com > gestionarea amenințărilor > politica > antispam > selectați Politica de filtrare antispam și politica de editare > proprietățile spam > Marcați ca spam > NDR prin mesaje > setați-l la "activat"**

Dacă credeți că un cont a fost compromis, consultați următoarele:

- [Răspunsul la un cont de E-mail compromis](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Eliminarea utilizatorilor blocați din portalul utilizatori restricționați din Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



