---
title: Swap vă clasic site-ul rădăcină, cu un site Modern
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270756"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap vă clasic site-ul rădăcină, cu un site Modern

În cazul în care mediul vostru a fost creat înainte de aprilie 2019, puteţi schimba site-ul rădăcină a unui site modern utilizând Microsoft PowerShell:

- Dacă aveţi un alt site pe care doriţi să o utilizaţi ca site-ul rădăcină, puteţi înlocui (swap) rădăcină site-ul cu ea. 
    - Utilizaţi [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locaţia de un site cu un alt site în timp ce site-ul original de arhivare. Disponibil pentru echipa site-ului (nu este conectat la un grup) şi de site-ul de comunicare. 

- Capabilităţi suplimentare vor fi introduse în curând care vă va permite să păstraţi folosind conţinut pe site-ul, dar conversia site-ul existent la un site de comunicare. 
>[!Important]
>Aceste capabilităţi va fi lansat treptat. Continuaţi pentru a verifica Office 365 centru de mesaje pentru actualizări. 

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu schimbarea site-uri

- Site-ul ţintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie el scotocit din nou pentru a actualiza indexul de căutare. Nu există nici un pas manuală necesară - acest lucru se va face automat.
- Nimic depinde şi de link-uri "statice" (cum ar fi fişiere fişier sincronizare și OneNote) va trebui să manual corectate.
- În cazul în care site-ul sursă a fost un site de ştiri organizaţionale, Actualizaţi URL-ul.Obţineţi o listă de toate site-urile de ştiri organizatorice.
- Proiect Server site-uri trebuie să fie validate pentru a se asigura că acestea sunt încă asociate corect.





