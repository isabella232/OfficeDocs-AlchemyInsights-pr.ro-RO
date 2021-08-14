---
title: Restaurarea unui grup de Microsoft 365 șters
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
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959038"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurarea unui grup de Microsoft 365 șters

Puteți restaura un grup de persoane Microsoft 365 ștergere sau un Microsoft Teams timp de 30 de zile de la ștergere.

1. Accesați the [Centru de administrare Microsoft 365 pentru](https://aka.ms/RestoreDeletedGroup) a vă conecta la o listă cu grupurile și echipele șterse.

    **Notă:** Conectați-vă utilizând contul care este atribuit administratorului entității găzduite sau rolului de administrator al grupurilor.

1. Selectați grupul de Microsoft 365/grupul de Teams restaurați și faceți clic pe **Restaurare grup.**

    Dacă grupul nu poate fi restaurat din cauza unei adrese SMTP conflictuale, utilizați următoarea comandă pentru a găsi obiectul care provoacă conflictul și eliminați adresa SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Notă:** În unele cazuri, poate dura 24 de ore pentru ca grupul și toate datele sale să fie restaurate.

    Pentru mai multe informații sau pentru a afla cum să restaurați grupuri utilizând PowerShell, consultați [Restaurarea unui grup Microsoft 365 șters.](https://go.microsoft.com/fwlink/?linkid=867802)