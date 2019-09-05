---
title: Site-ul modern ca site-ul rădăcină
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753916"
---
# <a name="modern-site-as-root-site"></a>Site-ul modern ca rădăcină site-ului

Am început să rollout o nouă facilitate care vă va permite să swap site-ul site-ul [clasic rădăcină cu un site modern](https://docs.microsoft.com/sharepoint/modern-root-site). Utilizați [Invoke-,](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original. Disponibil pentru ambele site-uri de echipă (nu sunt conectate la un grup) și site-ul de comunicare.

>[!Important]
> Nu ștergeți site-ul rădăcină clasic pentru a crea un site modern de comunicare. Acest lucru nu este acceptat de Microsoft. Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizație inaccesibile tuturor utilizatorilor, până când restaurați site-ul sau creați un site nou la același URL. Vom comunica această caracteristică prin intermediul centrului de mesaje. Trebuie să vă așteptați ca funcția să fie activată în curând în chiriaș.

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu schimbarea site-uri
- Site-ul țintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie scotocit din nou pentru a actualiza indexul de căutare. Nu există nici un pas manual necesar aici, acest lucru se va face în mod automat.
- Orice depinde de "static" link-uri (cum ar fi fișiere de sincronizare și fișiere OneNote) va trebui să fie corectate manual.
- Site-uri de proiect Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect. 
