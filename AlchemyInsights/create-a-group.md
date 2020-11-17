---
title: Crearea unui grup
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089173"
---
# <a name="create-a-group"></a>Crearea unui grup

Acest subiect descrie crearea grupurilor.

**Permisiunea de a crea un grup**

Asigurați-vă că sunteți autorizat să creați un grup nou. Administratorii globali pot dezactiva crearea grupurilor în portalul Azure sau în panoul de acces. Este posibil să aveți nevoie de un administrator pentru a crea noul grup sau pentru a vă oferi permisiuni corespunzătoare.

**Gestionarea permisiunilor de creare a grupurilor**

1. Administratorii globali pot gestiona permisiunile de creare a grupurilor (din motive legate de securitate) sau grupuri 365 Office create în portalul Azure sau în panoul de acces, alegând "utilizatorii pot crea grupuri de securitate în portaluri Azure" sau "utilizatorii pot crea grupuri Office 365 în portaluri Azure" opțiuni din **toate grupurile**  >  **generale (Setări)**.
2. De asemenea, puteți restricționa crearea grupurilor pentru a selecta un grup de utilizatori dacă aveți o licență Azure Active Directory P1 Premium.

**Dezactivarea notificării de întâmpinare pentru noii membri ai grupului Office 365**

Notificarea de bun venit trimisă utilizatorilor care sunt adăugați la Office 365 Groups poate fi dezactivată setând **UnifiedGroupWelcomeMessageEnabled** la false în PowerShell. Aflați mai multe despre această setare [aici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

