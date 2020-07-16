---
title: Probleme de licențiere Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148318"
---
# <a name="yammer-licensing-issues"></a>Probleme de licențiere Yammer

Toți utilizatorii trebuie să aibă o licență pentru a utiliza serviciul Yammer Enterprise, dar în mod implicit Yammer nu solicită ca utilizatorii să aibă o licență pentru a accesa serviciul. Când un administrator modifică setarea pentru a bloca utilizatorii Microsoft 365 fără licențe Yammer, utilizatorii cărora nu li se atribuie o licență Yammer Enterprise nu pot accesa serviciul Yammer. Pentru mai multe informații, consultați [Gestionarea licențelor de utilizator Yammer în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Când licențele sunt eliminate de la utilizatori, dala Yammer nu mai este afișată, iar alte servicii pot utiliza eliminarea licenței pentru a ascunde caracteristicile. În alte cazuri, caracteristicile pot apărea în continuare, dar necesită atribuirea licenței pentru a funcționa.  

**Licența nu se actualizează pentru utilizator**  

Ocazional, unui utilizator i se atribuie o licență, dar nu poate accesa Yammer. Întârzierile sunt mai susceptibile să apară atunci când o atribuire de licență în masă este în curs de desfășurare. Este posibil ca utilizatorii Yammer să nu fie actualizați în aceeași ordine în care licențele sunt modificate în Azure AD, deoarece sistemul se execută asincron. Așteptați până la 24 de ore înainte de a deschide un caz de asistență pentru a raporta problemele de sincronizare a licenței.  

**Cesiunea licenței în bloc**  

Licențele pot fi atribuite prin intermediul centrului de administrare sau al scripturilor PowerShell. Pentru mai multe informații, consultați [Atribuirea licențelor utilizatorilor](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) și [Atribuirea licențelor pentru conturile de utilizator cu Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Asistența Microsoft nu oferă asistență pentru crearea scripturilor, dar documentația pentru atribuirea licenței Yammer este disponibilă. Pentru mai multe informații, consultați [Gestionarea licențelor Yammer utilizând Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).