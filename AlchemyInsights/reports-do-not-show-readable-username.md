---
title: Rapoartele din Centru de administrare Microsoft 365 numele de utilizator nu se pot citi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316196"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapoartele din Centru de administrare Microsoft 365 numele de utilizator nu se pot citi

Rapoartele din Centru de administrare Microsoft 365 nu afișează nume de utilizator, însă afișează în schimb valori numerice alfa, cum ar fi B2BC6C15BB9FCDEA71E5CD302D228CC8.

Acesta este comportamentul așteptat și a fost comunicat în Centrul de mesaje (MC275344, publicat pe 3 august 2021). 

Administratorii globali pot reveni la această modificare pentru entitatea lor găzduită și pot afișa informații de identificare a utilizatorilor, dacă practicile de confidențialitate ale organizației lor permit acest lucru. Pentru a reveni la modificarea pentru entitatea găzduită:

1. În centrul de administrare, accesați **Setări**  >  **Org settings**  >  [**Services**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)și selectați **Reports**. 
1. Sub **Alegeți cum să afișați informațiile de** utilizator , **selectați Afișați informațiile de** utilizator care pot fi identificate în rapoarte , apoi rulați din nou raportul.