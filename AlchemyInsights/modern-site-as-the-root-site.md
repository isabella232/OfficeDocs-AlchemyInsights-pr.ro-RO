---
title: Site-ul modern ca site-ul rădăcină
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713803"
---
# <a name="modern-site-as-root-site"></a>Site-ul modern ca site-ul rădăcină

Am început să rollout o nouă caracteristică care vă va permite să [swap site-ul clasic rădăcină site-ul cu un site modern](https://docs.microsoft.com/sharepoint/modern-root-site). Utilizați [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu un alt site în timp ce arhivați site-ul original. Disponibil atât pentru site-ul de echipă (care nu este conectat la un grup), cât și pentru site-ul de comunicare.

>[!Important]
> Nu ștergeți site-ul rădăcină clasic pentru a crea un site de comunicare modern. Acest lucru nu este acceptat de Microsoft. Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizația dvs. Vom comunica această caracteristică prin intermediul centrului de mesaje. Ar trebui să vă așteptați ca caracteristica să fie activată în entitatea găzduită în scurt timp.

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu site-uri de schimbare
- Site-ul țintă poate returna o eroare "negăsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui recrawled pentru a actualiza indexul de căutare. Nu există nici un pas manual necesar aici, acest lucru se va face în mod automat.
- Orice lucru dependent de linkurile "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui corectat manual.
- Site-uri Project Server poate fi necesar să fie validate pentru a se asigura că acestea sunt încă asociate corect. 
