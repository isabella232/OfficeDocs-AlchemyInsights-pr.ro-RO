---
title: Remedierea politicii de entitate găzduită (înlocuire de acțiune)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695696"
---
# <a name="fix-tenant-policy-action-override"></a>Remedierea politicii de entitate găzduită (înlocuire de acțiune)

O politică anti-spam din entitatea găzduită a afectat acest mesaj. Pentru a revizui politica, procedați astfel:

1. Accesați centrul de [conformitate Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143), apoi accesați Politica de **gestionare a amenințărilor**  >    >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Verificați dacă sursa de **politică** indică următoarele:  **Adăugare-XHeader/ModifySubject/redirecționare/Ștergere/niciun mesaj de acțiune/CCI**

    Dacă da, pe fila **particularizat** , Verificați setările politicii care au afectat mesajul. Este posibil ca **setările standard** aplicate pentru toți clienții Exchange Online Protection să fi afectat mesajul.

Pentru mai multe informații despre configurarea politicilor de filtrare antispam, consultați [Configurarea politicilor de filtrare antispam](https://go.microsoft.com/fwlink/?linkid=2101431).
