---
title: Sincronizare hash parolă pentru serviciul de domeniu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177624"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sincronizare hash parolă pentru serviciul de domeniu

**Dacă instanța Azure AD DS vă solicită să activați sincronizarea codului hash pentru parole**

Întâlniți un scenariu în care se execută un mediu hibrid cu utilizatorii care se sincronizează dintr-un mediu Azure Active Directory (AD DS) local. Acest scenariu este întâlnit în ciuda faptului că aveți sincronizarea cu parola hash din AD DS local la entitatea găzduită Azure AD.

**Cauza**

Acest lucru se întâmplă deoarece Azure AD Connect în mod implicit nu sincronizează noile hash-uri de tehnologie LAN Manager (NTLM) și Kerberos password care sunt necesare pentru Azure AD DS.

**Soluție** 

Trebuie să configurați Azure AD Connect pentru a sincroniza acele parole hash necesare pentru autentificarea NTLM și Kerberos.

După ce Azure AD Connect este configurat, un eveniment local de creare a unui cont sau de modificare a parolei, de asemenea, sincronizează hash-ul de parolă moștenit la Azure AD. Vă rugăm să consultați [aici](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) pentru mai multe informații despre aceasta și pentru instrucțiuni despre cum să activați sincronizarea parolelor în medii hibride AZURE AD DS.