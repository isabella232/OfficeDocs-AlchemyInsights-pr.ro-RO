---
title: Actualizarea înregistrărilor DNS pentru a vă menține site-ul web la furnizorul de găzduire curent
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699531"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Actualizarea înregistrărilor DNS pentru a vă menține site-ul web la furnizorul de găzduire curent

1. În centrul de administrare Microsoft 365, accesați **Setup**  >  pagina[Domains](https://portal.office.com/adminportal/home#/Domains) setup și, în lista de domenii, selectați domeniul pe care îl utilizați pentru site-ul web.

2. Selectați **+ înregistrare particularizată nouă** și introduceți următoarele:

  - Pentru **tip DNS** , introduceți: **A (adresă)**

  - Pentru **nume gazdă sau alias**, tastați următoarele: **@**

  - Pentru **adresă IP**, tastați adresa IP statică pentru site-ul web unde este găzduit în prezent (de exemplu, 172.16.140.1).

    Aceasta trebuie să fie o adresă IP  *statică*  pentru site-ul web, nu o adresă IP  *dinamică*  . Consultați site-ul unde este găzduit site-ul web pentru a vă asigura că puteți obține o adresă IP statică pentru site-ul web public.

3. Selectați **Salvare**.

În plus, puteți să creați o înregistrare CNAME pentru a-i ajuta pe clienți să vă găsească site-ul web.
  
1. Selectați **+ înregistrare particularizată nouă** și introduceți următoarele:

  - Pentru **tip DNS** , introduceți: **CNAME (alias)**

  - Pentru **nume gazdă sau alias**, tastați următoarele: **www**

  - Pentru **adresă de puncte**, tastați numele de domeniu complet calificat (FQDN) pentru site-ul web (de exemplu, contoso.com).

2. Selectați **Salvare**.
