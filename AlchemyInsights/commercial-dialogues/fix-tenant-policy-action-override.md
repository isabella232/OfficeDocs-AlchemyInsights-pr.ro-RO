---
title: Remedierea politicii entității găzduite (înlocuire acțiune)
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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896087"
---
# <a name="fix-tenant-policy-action-override"></a>Remedierea politicii entității găzduite (înlocuire acțiune)

Una dintre politicile dvs. antispam a afectat acest mesaj. Pentru a examina politicile, urmați acești pași:

1. În portalul de Microsoft 365 Defender de la , accesați Trimiterea prin e-mail & a politicilor de colaborare & Reguli <https://security.microsoft.com/>  \>  \>  \> **antispam** în **secțiunea** Politici.

   Pentru a merge direct la **pagina Politici antispam,** utilizați <https://security.microsoft.com/antispam> .

2. Pe pagina Politici antispam, selectați politica, făcând clic pe numele politicii (Tipul  este Politica **antispam** particularizată sau Numele este politica de intrare antispam  **(implicit)**).
3. În meniul volant detalii care apare, selectați **Editare acțiuni** în **secțiunea** Acțiuni.
4. În **secțiunea Acțiuni mesaj,** revizuiți elementele pentru **Spam,** **Spam** de încredere maxim, **Phishing** și **Phishing** cu încredere ridicată pentru a vedea dacă este selectată oricare dintre următoarele valori:
   - **Adăugarea antetului X**
   - **Pregătirea liniei de subiect cu textul**
   - **Redirijați mesajul la adresa de e-mail**
   - **Ștergerea mesajului**
   - **Nicio acțiune**

   Este posibil ca setările **Standard aplicate tuturor** clienților Protecție Exchange Online să fi afectat mesajul.

Pentru mai multe informații, [consultați Configurarea politicilor antispam în EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
