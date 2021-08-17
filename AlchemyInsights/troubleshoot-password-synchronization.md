---
title: Depanarea sincronizării parolelor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105770"
---
# <a name="troubleshoot-password-synchronization"></a>Depanarea sincronizării parolelor

Pentru a depana problemele de sincronizare a parolelor, începeți prin a utiliza această activitate Conectare de depanare AAD pentru a afla de ce nu se sincronizează parolele. Pentru a începe, accesați Gestionarea [sincronizării directe](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Deschideți o nouă Windows PowerShell pe Azure AD Conectare server și selectați **opțiunea Executare ca** administrator.

2. Rulați Set-ExecutionPolicy RemoteSigned sau Set-ExecutionPolicy Nerestricționat.

3. Porniți Expertul de Conectare Azure AD.

4. Accesați pagina Activități suplimentare din Pagina > **Următorul**  >  **Depanare.**

5. **Selectați** Lansare pentru a deschide meniul de depanare PowerShell.

6. Selectați **Depanarea sincronizării parolelor.**

    Problema este de obicei faptul că nu este sincronizată o parolă pentru un anumit cont de utilizator.

    **Note** Sincronizarea parolelor nu reușește dacă ultima sincronizare cu succes a parolelor a fost cu ceva timp în urmă.

Pentru mai mult ajutor la depanarea sincronizării parolelor, consultați [Depanarea sincronizării parolelor hash cu Azure AD Conectare sincronizare.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)