---
title: Actualizați înregistrările DNS pentru a vă păstra site-ul web cu furnizorul curent de găzduire
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665772"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Actualizați înregistrările DNS pentru a vă păstra site-ul web cu furnizorul curent de găzduire

1. În centrul de administrare Microsoft 365, accesați pagina Domenii de **instalare**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) și, în lista de domenii, selectați domeniul pe care îl utilizați pentru site-ul dvs.

2. Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:

  - Pentru **tipul DNS** introduceți: **A (Adresă)**

  - Pentru **nume gazdă sau alias**, tastați următoarele:**@**

  - Pentru **adresa IP**, tastați adresa IP statică pentru site-ul web unde este găzduită în prezent (de exemplu, 172.16.140.1).

    Aceasta trebuie să fie o adresă IP *statică* pentru site-ul web, nu o adresă IP *dinamică.* Consultați site-ul unde este găzduit site-ul dvs., pentru a vă asigura că puteți obține o adresă IP statică pentru site-ul web public.

3. Selectați **Salvare**.

În plus, puteți crea o înregistrare CNAME pentru a ajuta clienții să vă găsească site-ul web.
  
1. Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:

  - Pentru **tipul DNS** introduceți: **CNAME (Alias)**

  - Pentru **nume gazdă sau alias**, tastați următoarele: **www**

  - Pentru **puncte de adresă,** tastați numele de domeniu complet calificat (FQDN) pentru site-ul web (de exemplu, contoso.com).

2. Selectați **Salvare**.
