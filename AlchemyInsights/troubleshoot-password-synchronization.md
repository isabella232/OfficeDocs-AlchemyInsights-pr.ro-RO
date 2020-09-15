---
title: Depanarea sincronizării parolei
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664938"
---
# <a name="troubleshoot-password-synchronization"></a>Depanarea sincronizării parolei

Pentru a depana problemele de sincronizare a parolei, începeți prin a utiliza această activitate de depanare AAD Connect pentru a determina de ce parolele nu se sincronizează. Pentru a începe, accesați [gestionare sincronizare directă](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Deschideți o nouă sesiune Windows PowerShell pe serverul Azure AD Connect și selectați opțiunea **Executare ca administrator** .

2. Rulează set-ExecutionPolicy RemoteSigned sau set-ExecutionPolicy nerestricționate.

3. Porniți Expertul Azure AD Connect.

4. Accesați pagina activități suplimentare > depanare în **Troubleshoot**  >  **continuare**.

5. Selectați **lansare** pentru a deschide meniul depanare PowerShell.

6. Selectați **depanați sincronizarea parolelor**.

    Problema este, de obicei, că o parolă nu este sincronizată pentru un anumit cont de utilizator.

    **Note** Sincronizarea parolelor nu reușește dacă Ultima sincronizare cu parolă reușită a fost acum ceva timp.

Pentru mai mult ajutor la depanarea sincronizării parolei, consultați [Depanarea sincronizării hash a parolei cu sincronizarea AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).