---
title: Depanarea sincronizării parolei
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387889"
---
# <a name="troubleshoot-password-synchronization"></a>Depanarea sincronizării parolei

Pentru a depana problemele de sincronizare a parolei, începeți prin a utiliza această activitate de depanare AAD Connect pentru a determina de ce parolele nu se sincronizează. Pentru a începe, [accesați Gestionare sincronizare directă](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Deschideți o nouă sesiune Windows PowerShell pe serverul Azure AD Connect și selectați opțiunea **Executare ca administrator.**

2. Executați Set-ExecutionPolicy RemoteSigned sau Set-ExecutionPolicy Nerestricționat.

3. Porniți expertul Azure AD Connect.

4. Accesați pagina Activități suplimentare > **Depanare**  >  **următoare**.

5. Selectați **Lansare** pentru a deschide meniul de depanare PowerShell.

6. Selectați **Depanare sincronizare parolă**.

    Problema este, de obicei, că o parolă nu este sincronizat pentru un anumit cont de utilizator.

    **Note** Sincronizarea parolei nu reușește dacă ultima sincronizare reușită a parolei a fost cu ceva timp în urmă.

Pentru mai mult ajutor pentru depanarea sincronizării parolei, consultați [Depanarea sincronizării hash a parolei cu sincronizarea Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).