---
title: Probleme cu licențierea Yammer
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657288"
---
# <a name="yammer-licensing-issues"></a>Probleme cu licențierea Yammer

Toți utilizatorii trebuie să aibă o licență pentru a utiliza serviciul Yammer Enterprise, dar în mod implicit Yammer nu necesită ca utilizatorii să aibă o licență pentru a accesa serviciul. Atunci când un administrator modifică setarea pentru a bloca utilizatorii Microsoft 365 fără licențe Yammer, utilizatorii cărora nu li s-a atribuit o licență Yammer Enterprise nu pot accesa serviciul Yammer. Pentru mai multe informații, consultați [gestionarea licențelor de utilizator Yammer în Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Atunci când licențele sunt eliminate din utilizatori, dala Yammer nu mai este afișată și alte servicii pot utiliza eliminarea licențelor pentru a ascunde caracteristicile. În alte cazuri, caracteristicile pot apărea în continuare, dar necesită atribuirea licenței pentru a funcționa.  

**Licența nu se actualizează pentru utilizator**  

Ocazional, unui utilizator i se atribuie o licență, dar încă nu poate accesa Yammer. Întârzierile sunt mai susceptibile să apară atunci când este în curs o atribuire a licenței în masă. Este posibil ca utilizatorii Yammer să nu fie actualizați în aceeași ordine ca licențele să fie schimbate în Azure AD, deoarece sistemul rulează asincron. Așteptați până la 24 de ore înainte de a deschide un caz de asistență pentru a raporta problemele de sincronizare a licențelor.  

**Atribuirea de licențe în masă**  

Licențele pot fi atribuite prin centrul de administrare sau prin scriptarea PowerShell. Pentru mai multe informații, consultați [atribuirea de licențe pentru utilizatori](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) și [atribuirea de licențe conturilor de utilizator cu Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Asistența Microsoft nu oferă asistență pentru crearea de scripturi, dar documentația despre atribuirea licenței Yammer este disponibilă. Pentru mai multe informații, consultați [gestionarea licențelor Yammer utilizând Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).