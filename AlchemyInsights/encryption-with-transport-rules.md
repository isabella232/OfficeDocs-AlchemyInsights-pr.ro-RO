---
title: Criptarea cu regulile de transport
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915168"
---
# <a name="encryption-with-transport-rules"></a>Criptarea cu regulile de transport

În [Centrul de administrare Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) puteți utiliza capacitățile Office Message Encryption (OME) în regulile de flux de corespondență pentru a declanșa criptarea mesajelor. Alegeți opțiunea **Aplicați Office 365 Message Encryption și protejarea drepturilor** din condiția Regulă de transport.

- Pentru mai multe informații, consultați [Definirea regulii de flux de corespondență pentru criptare](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- În PowerShell, utilizați cmdletul [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) și setați parametrul *ApplyOME* la $true.
