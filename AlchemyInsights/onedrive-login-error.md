---
title: Eroare de conectare la OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982543"
---
# <a name="onedrive-login-error-aadsts50011"></a>Eroare de conectare la OneDrive AADSTS50011

Dacă primiți o eroare "AADSTS50011: adresa URL de răspuns specificată în solicitare nu se potrivește cu răspunsul" atunci când vă conectați la aplicația OneDrive, verificați următoarele:

Versiunea dumneavoastră OneDrive trebuie să fie egală cu sau mai mare decât versiunea 20.052. XXXX. XXXX. Pentru a vă verifica versiunea, faceți clic pe pictograma OneDrive albastră din zona de notificare, selectați **ajutor & setări > setări >**.

Este posibil ca rețeaua să blocheze traficul către **g.live.com** și **oneclient.SFX.MS**. Dacă traficul este blocat, OneDrive nu se poate actualiza singur. Lucrați cu administratorul de rețea pentru a vă asigura că aveți acces la acele URL-uri. [Aceste puncte finale](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) ar trebui să fie accesibile pentru clienții care utilizează Microsoft 365 planuri.

Dacă trebuie să obțineți manual o versiune curentă de OneDrive, vizitați [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
