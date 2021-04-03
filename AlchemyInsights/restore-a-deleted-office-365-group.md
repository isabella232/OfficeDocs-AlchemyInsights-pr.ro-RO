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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505699"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Restaurarea unui grup Microsoft 365 șters

Puteți restaura un grup Microsoft 365 șters sau Microsoft Teams în termen de 30 de zile de la ștergere.

1. Pentru a vă conecta la centrul de administrare Microsoft 365 și a lista grupurile și echipele șterse, accesați Centrul de [administrare Microsoft 365](https://aka.ms/RestoreDeletedGroup).

    **Notă:** Conectați-vă utilizând contul care este atribuit administratorului entității găzduite sau rolului de administrator al grupurilor.

1. Selectați grupul Microsoft 365 șters/Teams pentru a fi restaurat și dați clic pe **Restabiliți grupul**.

    Dacă grupul nu poate fi restaurat din cauza unei adrese SMTP conflictuale, utilizați următoarea comandă pentru a găsi obiectul care provoacă conflictul și eliminați adresa SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Notă:** În unele cazuri, poate dura 24 de ore pentru ca grupul și toate datele sale să fie restaurate.

    Pentru mai multe informații sau pentru a afla cum să restaurați grupuri utilizând PowerShell, consultați [Restaurarea unui grup Microsoft 365 șters.](https://go.microsoft.com/fwlink/?linkid=867802)