---
title: Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353189"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Actualizarea înregistrărilor DNS pentru a menţine site-ul dvs cu furnizorul de găzduire curent

1. În pagina [domenii](https://portal.office.com/adminportal/home#/Domains) , în lista de domenii, selectaţi domeniul utilizaţi pentru site-ul dumneavoastră, şi apoi selectaţi **Setări DNS** în panoul de administrare.

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
