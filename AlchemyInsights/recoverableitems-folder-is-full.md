---
title: folderul RecoverableItems 1336 este plin
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741279"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folderul Elemente recuperabile este plin

Pentru cutiile poștale Exchange Online, limita implicită de stocare pentru folderul Elemente recuperabile este 30 GB. Limita de stocare pentru folderul Elemente recuperabile este mărită automat la 100 GB dacă cutia poștală este plasată în așteptare pentru litigii, descoperire eDiscovery sau este atribuită unei politici de retenție.

Atunci când folderul Elemente recuperabile atinge limita de stocare, funcționalitatea cutiei poștale este afectată în următoarele moduri:

- Utilizatorul nu poate șterge elemente din cutia poștală.

- Asistentul pentru foldere gestionate nu poate șterge elemente pe baza etichetei de retenție sau a setărilor de folder gestionate.

- Pentru cutiile poștale care au activată recuperarea unui singur element sau sunt plasate în așteptare, procesul de protecție a paginilor de copiere-la-scriere nu poate menține versiunile de elemente editate de utilizator.

- Pentru cutiile poștale care au activată înregistrarea în jurnal a auditării cutiilor poștale, nu se pot salva intrări în jurnal de auditare în caseta de auditare din folderul Elemente recuperabile.

Pentru cutiile poștale care nu sunt în așteptare, administratorii pot utiliza `Search-Mailbox -SearchDumpsterOnly -DeleteContent` comanda în Exchange Online PowerShell pentru a șterge elemente din folderul Elemente recuperabile. Pentru informații suplimentare, consultați următoarele articole:

- [Căutarea și ștergerea mesajelor](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Căutare-cutie poștală](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pentru cutiile poștale care sunt în așteptare, administratorii trebuie să elimine suspendarea înainte să poată șterge elemente din folderul Elemente recuperabile. Pentru mai multe informații, consultați [ștergerea elementelor din folderul Elemente recuperabile din cutiile poștale bazate pe cloud în așteptare](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Pentru a preveni ca folderul Elemente recuperabile să devină plin, administratorii pot mări limita de stocare a folderului Elemente recuperabile pentru cutiile poștale în așteptare și să configureze o politică de retenție a cutiei poștale care mută elementele din folderul Elemente recuperabile în cutia poștală de arhivă a utilizatorului. Consultați [creșterea cotei de Elemente recuperabile pentru cutiile poștale în așteptare](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
