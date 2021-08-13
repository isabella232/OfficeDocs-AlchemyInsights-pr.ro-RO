---
title: Despre identitatea din Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918949"
---
# <a name="about-identity-in-yammer"></a>Despre identitatea din Yammer

Se recomandă ca toate rețelele să aibă următorii pași pentru a evita problemele legate de identitate:

1. Impuneți Office 365 după asigurarea accesului la conturile Microsoft 365 pentru utilizatorii din Azure AD, pentru a vă asigura că toți utilizatorii se autentifică utilizând contul de e-Microsoft 365 principal. Pentru mai multe informații, consultați [Office 365 identităților pentru Yammer utilizatori.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Sintetizarea mai multor Yammer rețea. Configurațiile Yammer moștenite permit mai multor rețele Yammer să fie conectate la o singură entitate găzduită. Pentru mai multe informații, consultați [Migrarea rețelei - Sintetizarea mai multor Yammer rețea.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Opțional, impuneți licențierea Yammer a bloca posibilitatea utilizatorilor de Yammer dacă aceștia nu au o licență. Pentru mai multe informații, [consultați Yammer licențelor de utilizator în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. În sfârșit, auditați lista de utilizatori pentru rețelele Yammer vechi și suspendați utilizatorii moșteniți. Se recomandă să suspendați (să dezactivați) utilizatorii în loc să-i ștergeți, deoarece ștergerea este ireversibilă. Pentru mai multe informații, consultați [Auditarea utilizatorilor Yammer din rețelele conectate la Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) și [Eliminarea utilizatorilor.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Prin configurarea Yammer utilizând acești pași, veți fi, de asemenea, gata să configurați rețeaua Yammer pentru Modul nativ pentru Microsoft 365. Pentru mai multe informații, [consultați Configurarea rețelei Yammer nativă pentru modul nativ pentru Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).