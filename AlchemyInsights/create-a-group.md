---
title: Crearea unui grup
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929317"
---
# <a name="create-a-group"></a>Crearea unui grup

Acest subiect descrie crearea de grupuri.

**Permisiunea de a crea un grup**

Asigurați-vă că sunteți autorizat să creați un grup nou. Administratorii globali pot dezactiva crearea grupurilor în portalul Azure sau în panoul Access. Poate fi necesar ca un administrator să creeze noul grup pentru dvs. sau să vă ofere permisiunile corespunzătoare.

**Gestionarea permisiunilor de creare a grupurilor**

1. Administratorii globali pot gestiona permisiunile de creare a grupurilor (din motive de securitate) sau grupurile Office 365 create în portalul Azure sau în panoul de acces, alegând opțiunile "Utilizatorii pot crea grupuri de securitate în portaluri Azure" sau "Utilizatorii pot crea grupuri Office 365 în portaluri Azure" în Toate grupurile   >  **General (Setări).**
2. De asemenea, puteți restricționa crearea de grupuri pentru a selecta un grup de utilizatori dacă aveți o licență Azure Active Directory P1 Premium grup.

**Dezactivarea notificării de bun venit pentru Office 365 grupului nou**

Notificarea de bun venit trimisă utilizatorilor care sunt adăugate la grupurile Office 365 poate fi dezactivată prin setarea **UnifiedGroupGroupcomeMessageEnabled** la False în Powershell. Aflați despre această setare [aici.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

