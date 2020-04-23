---
title: Depanarea sincronizării parolei
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732522"
---
# <a name="troubleshoot-password-synchronization"></a>Depanarea sincronizării parolei

Pentru a depana problemele în cazul în care nu există parole sincronizate cu Azure AD Conectați versiunea 1.1.614.0 sau o versiune ulterioară:
  
1. Deschideți o nouă sesiune Windows PowerShell pe serverul Azure AD Connect cu opțiunea **Executare ca Administrator.**

2. Executare **set-executionPolicy RemoteSigned** sau **Set-ExecutionPolicy nerestricționat**.

3. Porniți expertul Azure AD conecta.

4. Navigați la pagina **Activități suplimentare,** selectați **Depanare**și faceți clic pe **Următorul**.

5. În pagina Depanare, faceți clic pe **Lansare pentru a porni meniul de depanare** în PowerShell.

6. În meniul principal, selectați **Depanare sincronizare parolă**.

7. În meniul sub, selectați **Sincronizare parolă nu funcționează deloc**.

**Înțelegerea rezultatelor activității de depanare**
  
Activitatea de depanare efectuează următoarele verificări:
  
- Validează că caracteristica de sincronizare a parolei este activată pentru entitatea găzduită Azure AD.

- Validează că serverul Azure AD Connect nu este în modul de așteptare.

- Pentru fiecare conector Active Directory local existent (care corespunde unei păduri Active Directory existente):

- 
  - Validează că este activată caracteristica de sincronizare a parolei.

  - Caută evenimente de sincronizare a parolei în jurnalele de evenimente de eveniment aplicație Windows.

  - Pentru fiecare domeniu Active Directory sub conectorul Active Directory local:

  - Validează că domeniul este accesibil de pe serverul Azure AD Connect.

  - Validează că conturile active Directory Domain Services (AD DS) utilizate de conectorul Active Directory local are numele de utilizator, parola și permisiunile necesare pentru sincronizarea parolei.

Pentru mai multe ajutor depanarea sincronizarea parolei, consultați [Depanarea sincronizării parolei cu sincronizarea Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  