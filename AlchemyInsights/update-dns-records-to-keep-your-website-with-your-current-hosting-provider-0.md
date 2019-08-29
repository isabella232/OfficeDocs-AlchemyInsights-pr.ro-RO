---
title: Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665772"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent

1. În centrul de administrare Microsoft 365, du-te la **Setup** > [domenii](https://portal.office.com/adminportal/home#/Domains) pagină și selectați din lista de domenii, domeniu care îl utilizaţi pentru site-ul dvs.

2. Selectaţi **+ nou record personalizat** şi introduceţi următoarele:

  - Pentru **tip DNS** intra: **(adresa)**

  - Pentru **gazdă nume sau Alias**, tastaţi următoarele:**@**

  - Pentru **Adresa IP**, tastaţi adresa IP statică pentru site-ul dvs., în cazul în care este în prezent găzduit (de exemplu, 172.16.140.1).

    Acest lucru trebuie să fie o adresă IP *statică* pentru site-ul, nu o adresă IP *dinamică* . Consultaþi site-ul unde este gazduit site-ul dvs să vă asiguraţi că puteţi obţine o adresă IP statică pentru site-ul dumneavoastră publice.

3. Selectaţi **Salvare**.

În plus, creaţi o înregistrare CNAME pentru a ajuta clienţii găsi site-ul dvs.
  
1. Selectaţi **+ nou record personalizat** şi introduceţi următoarele:

  - Pentru **tip DNS** intra: **CNAME (Alias)**

  - Pentru **gazdă nume sau Alias**, tastaţi următoarele: **www**

  - Pentru **puncte la adresă**, tastaţi numele de domeniu complet (FQDN) pentru site-ul web (de exemplu, contoso.com).

2. Selectaţi **Salvare**.
