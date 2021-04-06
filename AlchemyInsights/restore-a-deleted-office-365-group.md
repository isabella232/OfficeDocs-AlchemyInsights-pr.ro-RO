---
title: Restaurarea unui grup Microsoft 365 șters
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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597455"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurarea unui grup Microsoft 365 șters

Puteți restaura un grup Microsoft 365 șters sau Microsoft Teams în termen de 30 de zile de la ștergere.

1. Accesați Centrul de [administrare Microsoft 365 pentru a vă](https://aka.ms/RestoreDeletedGroup) conecta și a lista grupurile și echipele șterse.

    **Notă:** Conectați-vă utilizând contul care este atribuit administratorului entității găzduite sau rolului de administrator al grupurilor.

1. Selectați grupul Microsoft 365 șters/Teams pentru a fi restaurat și dați clic pe **Restabiliți grupul**.

    Dacă grupul nu poate fi restaurat din cauza unei adrese SMTP conflictuale, utilizați următoarea comandă pentru a găsi obiectul care provoacă conflictul și eliminați adresa SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Notă:** În unele cazuri, poate dura 24 de ore pentru ca grupul și toate datele sale să fie restaurate.

    Pentru mai multe informații sau pentru a afla cum să restaurați grupuri utilizând PowerShell, consultați [Restaurarea unui grup Microsoft 365 șters.](https://go.microsoft.com/fwlink/?linkid=867802)