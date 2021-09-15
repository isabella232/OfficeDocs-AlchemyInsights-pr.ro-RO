---
title: Rapoartele din Centrul de administrare Microsoft 365 nu afișează un nume de utilizator lizibil
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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327826"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapoartele din Centrul de administrare Microsoft 365 nu afișează un nume de utilizator lizibil

Rapoartele din Centrul de administrare Microsoft 365 nu afișează nume de utilizator, ci valori alfanumerice, cum ar fi B2BC6C15BB9FCDEA71E5CD302D228CC8.

Acesta este comportamentul așteptat și a fost comunicat în Centrul de mesaje (MC275344, publicat pe 3 august 2021). 

Administratorii globali pot anula această modificare pentru entitatea lor găzduită și pot afișa informații de identificare a utilizatorilor, dacă practicile de confidențialitate ale organizației permit acest lucru. Pentru a anula modificarea pentru entitatea găzduită:

1. În Centrul de administrare, accesați **Setări** > **Setări organizație** > [**Servicii**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) și selectați **Rapoarte**. 
1. Sub **Alegeți cum să afișați informațiile utilizatorului**, selectați **Afișați în rapoarte informațiile de identificare a utilizatorilor**, apoi rulați din nou raportul.