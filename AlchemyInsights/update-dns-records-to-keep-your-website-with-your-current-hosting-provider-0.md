---
title: Actualizarea înregistrărilor DNS pentru a menține furnizorul curent de găzduire al site-ului web
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007694"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Actualizarea înregistrărilor DNS pentru a menține furnizorul curent de găzduire al site-ului web

1. În lista Centru de administrare Microsoft 365, accesați pagina **Setup** Domains (Configurare domenii) și, în lista de domenii, selectați domeniul pe care îl utilizați  >  [](https://admin.microsoft.com/Adminportal#/Domains) pentru site-ul dvs. web.

2. Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:

  - Pentru **Tip DNS,** introduceți: **A (Adresă)**

  - Pentru **Nume gazdă sau Alias,** tastați următoarele: **@**

  - Pentru **Adresă IP**, tastați adresa IP statică pentru site-ul dvs. web unde este găzduit în prezent (de exemplu, 172.16.140.1).

    Aceasta trebuie să fie o adresă IP  *statică*  pentru site-ul web, nu o  *adresă*  IP dinamică. Consultați site-ul în care este găzduit site-ul web, pentru a vă asigura că puteți obține o adresă IP statică pentru site-ul web public.

3. Selectați **Salvare**.

În plus, puteți crea o înregistrare CNAME pentru a-i ajuta pe clienți să vă găsească site-ul web.
  
1. Selectați **+ Înregistrare particularizată nouă** și introduceți următoarele:

  - Pentru **Tip DNS introduceți:** **CNAME (Alias)**

  - Pentru **Nume gazdă sau Alias,** tastați următoarele: **www**

  - Pentru **Adresă indicatială,** tastați numele de domeniu complet calificat (FQDN) pentru site-ul web (de exemplu, contoso.com).

2. Selectați **Salvare**.
