---
title: Alerts missing from Alerts tab
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454969"
---
# <a name="alerts-missing-from-alerts-tab"></a>Alerts missing from Alerts tab

Fila **Avertizări funcționează** pe baza politicilor de configurare și activate din portalul Administrare aplicații din entitatea găzduită. De asemenea, politicile in-the-box în Guvernanța aplicațiilor trebuie să fie activate pentru a permite semnalelor să curgă în **fila** Avertizări. 

Confirmați că a fost generată avertizarea:

1. Accesați Politicile de guvernanță [a aplicațiilor](https://compliance.microsoft.com/m365appprotection?viewid=policies) și confirmați că ați creat cel puțin o politică de auditare sau activă.

1. Selectați politica și apoi selectați **Editare în** panoul volant. 

1. Verificați configurația politicii pentru a confirma că ar fi trebuit să fie generată o avertizare pe baza unui eveniment de politică inițiat cu mai mult de 24 de ore în urmă.

Pentru mai multe informații despre avertizările din Guvernanța aplicațiilor, consultați Începeți lucrul cu [detectarea și remedierea amenințărilor la aplicații.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)