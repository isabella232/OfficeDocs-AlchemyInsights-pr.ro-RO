---
title: 1336 RecoverableItems folder is full
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061768"
---
# <a name="the-recoverable-items-folder-is-full"></a>Folderul Elemente recuperabile este plin

Pentru Exchange Online poștale, limita implicită de stocare pentru folderul Elemente recuperabile este de 30 GB. Limita de stocare pentru folderul Elemente recuperabile crește automat la 100 GB în cazul în care cutia poștală este plasată în Reținere pe motiv de litigiu, reținere în depozit pentru descoperirea informațiilor electronic sau este atribuită unei politici de retenție.

Atunci când folderul Elemente recuperabile atinge limita de spațiu de stocare, funcționalitatea cutiei poștale este afectată în următoarele moduri:

- Utilizatorul nu poate șterge elemente din cutia poștală.

- Asistentul folder gestionat nu poate șterge elemente pe baza setărilor de etichetă de retenție sau de folder gestionat.

- Pentru cutiile poștale care au recuperare element unic activată sau sunt plasate în așteptare, procesul de protecție a paginii de copiere-la-scriere nu poate menține versiuni ale elementelor editate de utilizator.

- Pentru cutiile poștale care au activată înregistrarea în jurnalul de auditare a cutiilor poștale, nu se pot salva intrări din jurnalul de auditare a cutiilor poștale în subfolderul Auditări din folderul Elemente recuperabile.

Pentru cutiile poștale care nu sunt în așteptare, administratorii pot utiliza comanda din Exchange Online PowerShell pentru a șterge elementele din folderul `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Elemente recuperabile. Pentru informații suplimentare, consultați următoarele articole:

- [Căutarea și ștergerea mesajelor](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pentru cutiile poștale care sunt în așteptare, administratorii trebuie să elimine așteptarea înainte ca aceștia să poată șterge elemente din folderul Elemente recuperabile. Pentru mai multe informații, [consultați Ștergerea elementelor din folderul Elemente recuperabile din cutiile poștale bazate pe cloud care sunt în așteptare.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Pentru a împiedica deveni complet folderul de elemente recuperabile, administratorii pot mări limita de spațiu de stocare al folderului de elemente recuperabile pentru cutiile poștale în așteptare și pot configura o politică de retenție pentru cutia poștală ce mută elemente din folderul Elemente recuperabile în cutia poștală de arhivă a utilizatorului. Consultați [Creșterea cotei de elemente recuperabile pentru cutiile poștale în așteptare.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
