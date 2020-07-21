---
title: Ștergerea utilizatorului orfan de pe serverul local
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198590"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Ștergerea utilizatorului orfan de pe serverul local

Pentru a elimina un utilizator orfan, urmați acești pași:

1. Forțați sincronizarea directorului urmând instrucțiunile din [Ce este identitatea hibridă cu Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Pentru a verifica sincronizarea directorului, consultați [Ce este identitatea hibridă cu Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Dacă sincronizarea funcționează corect, dar ștergerea obiectului Active Directory nu se propagă în Azure AD, eliminați manual obiectul orfan utilizând unul dintre următoarele module Azure Active Directory pentru cmdlet-urile Windows PowerShell:

    Eliminare-MsolContact  
    Eliminare-MsolGroup  
    Eliminare-MsolUser

    De exemplu, pentru a elimina ID-ul de utilizator orfan john.smith@contoso.com, creat inițial utilizând sincronizarea directorului, executați cmdlet::

    Eliminare-MsolUser –UserPrincipalName John.Smith@Contoso.com