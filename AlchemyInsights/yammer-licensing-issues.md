---
title: Yammer de licențiere
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989747"
---
# <a name="yammer-licensing-issues"></a>Yammer de licențiere

Toți utilizatorii trebuie să aibă o licență pentru a utiliza serviciul Yammer Enterprise, dar, în mod Yammer implicit, nu necesită ca utilizatorii să aibă o licență pentru a accesa serviciul. Atunci când un administrator modifică setarea de Microsoft 365 bloca utilizatorii fără licențe Yammer, utilizatorii neaslocați unei licențe Yammer Enterprise nu pot accesa serviciul Yammer. Pentru mai multe informații, [consultați Yammer licențelor de utilizator în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Atunci când sunt eliminate licențe din utilizatori, dala Yammer nu mai este afișată și alte servicii pot utiliza eliminarea licenței pentru a ascunde caracteristicile. În alte cazuri, caracteristicile pot apărea încă, dar pot necesita atribuirea licențelor pentru operare.  

**Licența nu se actualizează pentru utilizator**  

Ocazional, unui utilizator i se atribuie o licență, dar tot nu poate accesa Yammer. Întârzierile sunt mai probabil să apară atunci când este în curs de desfășurare o atribuire a licenței în masă. Yammer posibil ca utilizatorii să nu fie actualizați în aceeași ordine ca licențele pe care le-au modificat în Azure AD, deoarece sistemul rulează asincron. Așteptați până la 24 de ore înainte de a deschide un caz de asistență pentru a raporta problemele de sincronizare a licenței.  

**Atribuirea în masă a licențelor**  

Licențele pot fi atribuite prin centrul de administrare sau scriptarea PowerShell. Pentru mai multe informații, [consultați Atribuirea de licențe utilizatorilor](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) și [Atribuirea de licențe conturilor de utilizator cu Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Asistența Microsoft nu oferă asistență pentru crearea de scripturi, dar documentația pentru atribuirea Yammer licențe este disponibilă. Pentru mai multe informații, [consultați Yammer licențelor utilizând Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).