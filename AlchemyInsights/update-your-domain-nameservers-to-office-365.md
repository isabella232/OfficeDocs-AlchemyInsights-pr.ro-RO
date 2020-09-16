---
title: Actualizarea serverelor de nume de domeniu pentru a indica la Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734923"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Actualizarea serverelor de nume de domeniu pentru a indica la Microsoft

Notă: Propagarea modificărilor pentru serverele de nume poate dura uneori până la 48 de ore.
  
Pentru a vă configura domeniul cu Microsoft, trebuie să actualizați serverele de nume de la registrator. Creați sau editați înregistrările serverului de nume în registratorul de domeniu.
  
1. Accesați site-ul web al registratorului de domeniu și găsiți zona în care puteți să editați serverele de nume.

2. Creați sau editați două înregistrări ale serverului de nume pentru a se potrivi cu aceste valori:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Salvați modificările.

De asemenea, puteți găsi instrucțiuni detaliate în acest articol: modificarea serverelor [de nume pentru a configura Microsoft 365 cu orice registrator de domeniu](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  