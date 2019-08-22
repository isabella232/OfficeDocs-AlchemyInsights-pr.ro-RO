---
title: Depanarea sincronizarea parolelor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533819"
---
# <a name="troubleshoot-password-synchronization"></a>Depanarea sincronizarea parolelor

Pentru a depana probleme în cazul în care parolele nu sunt sincronizate cu Azure AD conecta versiunea 1.1.614.0 sau o versiune ulterioară:
  
1. Deschideti o noua sesiune de Windows PowerShell pe serverul AD Azure Connect cu opţiunea de **a alerga as Administrator** .

2. Executați **Set-ExecutionPolicy RemoteSigned** sau **Set-ExecutionPolicy nerestricționată**.

3. Porni Expertul Azure AD Connect.

4. Navigați la **Sarcini suplimentare** , selectaţi **Depanarea**şi faceţi clic pe **Următorul**.

5. Pagina de depanare, faceţi clic pe meniul de **lansare pentru a începe depanarea** în PowerShell.

6. În meniul principal, selectaţi **Depanarea sincronizarea parolelor**.

7. În sub-meniu, selectaţi **sincronizarea parolelor nu funcţionează deloc**.

**Intelege rezultatele misiunii depanare**
  
Sarcina depanare efectuează următoarele verificări:
  
- Validează că funcţia de sincronizare parolare este activată pentru chiriaşul dumneavoastră azuriu AD.

- Validează că Azure AD Connect server nu este în modul de așteptare.

- Pentru fiecare existente local Active Directory connector, (care corespunde la o pădure Active Directory existente):

- 
  - Validează faptul că este activată caracteristica de sincronizare parola.

  - Căutările pentru parola sincronizare emoţie evenimente în jurnalele de evenimente de aplicaţie Windows.

  - Pentru fiecare domeniu Active Directory în conectorul de Active Directory local:

  - Validează că domeniul este accesibilă de pe serverul AD Azure Connect.

  - Validează că serviciile de domeniu Active Directory (AD DS) conturile utilizate de conectorul de Active Directory local are corect numele de utilizator, parola şi permisiunile necesare pentru sincronizarea parolelor.

Pentru mai mult ajutor parola sincronizare de depanare, consultaţi [Depanarea sincronizarea parolelor cu Azure AD conecta sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  