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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816371"
---
# <a name="create-a-group"></a>Crearea unui grup

Acest subiect descrie crearea de grupuri.

**Permisiunea de a crea un grup**

Asigurați-vă că sunteți autorizat să creați un grup nou. Administratorii globali pot dezactiva crearea grupurilor în portalul Azure sau în panoul Access. Poate fi necesar ca un administrator să creeze noul grup pentru dvs. sau să vă ofere permisiunile corespunzătoare.

**Gestionarea permisiunilor de creare a grupurilor**

1. Administratorii globali pot gestiona permisiunile de creare a grupurilor (din motive de securitate) sau grupurile Office 365 create în portalul Azure sau în panoul de acces, alegând opțiunile "Utilizatorii pot crea grupuri de securitate în portaluri Azure" sau "Utilizatorii pot crea grupuri Office 365 în portaluri Azure" în Toate grupurile   >  **General (Setări).**
2. De asemenea, puteți restricționa crearea de grupuri pentru a selecta un grup de utilizatori dacă aveți o licență Azure Active Directory P1 Premium.

**Dezactivarea notificării de bun venit pentru noii membri ai grupului Office 365**

Notificarea de bun venit trimisă utilizatorilor care sunt adăugate la grupurile Office 365 poate fi dezactivată prin setarea **UnifiedGroupWelcomeMessageEnabled** la False în Powershell. Aflați despre această setare [aici.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

