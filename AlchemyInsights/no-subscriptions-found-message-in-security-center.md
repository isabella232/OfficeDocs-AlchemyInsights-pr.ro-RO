---
title: Nu s-a găsit niciun mesaj de abonament în Centrul de securitate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544120"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Nu s-a găsit niciun mesaj de abonament în Centrul de securitate

Dacă în timp ce accesați Centrul de securitate Microsoft Defender obțineți un mesaj "Nu s-au găsit abonamente", înseamnă că Azure Active Directory (AAD) utilizat pentru a conecta utilizatorul la portal nu are o licență Microsoft Defender ATP.  

Tipul Windows licențele E5 Office E5 sunt licențe separate.

Deschideți un caz de asistență dacă licența a fost achiziționată, dar nu a fost asigurată pentru această instanță AAD. Fie aveți: <br/>
-   O posibilă problemă de asigurare a accesului pentru licențe.<br/>
-   Din greșeală, asigurarea accesului la licența către alt Microsoft AAD decât cel utilizat pentru autentificare în serviciu.