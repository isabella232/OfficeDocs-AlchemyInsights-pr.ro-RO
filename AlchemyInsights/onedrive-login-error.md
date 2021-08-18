---
title: OneDrive eroare de conectare AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112924"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive eroare de conectare AADSTS50011

Dacă primiți eroarea "AADSTS50011: URL-ul de răspuns specificat în solicitare nu corespunde răspunsului" atunci când vă conectați la aplicația OneDrive, căutați următoarele:

Versiunea OneDrive trebuie să fie egală cu sau mai mare decât versiunea 20.052.XXXX.XXXX. Pentru a verifica versiunea, faceți clic pe pictograma OneDrive albastră din zona de notificare, **selectați Ajutor & Setări > Setări > Despre**.

Rețeaua dvs. poate bloca traficul **pentru a g.live.com** și **oneclient.sfx.ms**. Dacă traficul este blocat, nu OneDrive să se actualizeze singur. Lucrați cu administratorul de rețea pentru a vă asigura că aveți acces la acele URL-uri. [Aceste puncte finale trebuie să](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) fie accesibile pentru clienții care utilizează Microsoft 365 planuri.

Dacă trebuie să obțineți manual o versiune curentă de OneDrive, vizitați [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
