---
title: Site modern ca site rădăcină
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666882"
---
# <a name="modern-site-as-root-site"></a>Site modern ca site rădăcină

Am început să lansăm o nouă caracteristică care vă va permite să vă swap site-ul de [rădăcină clasic site cu un site modern](https://docs.microsoft.com/sharepoint/modern-root-site). Utilizați [invocare-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locația unui site cu alt site în timp ce arhivați site-ul original. Disponibil pentru ambele site-uri de echipă (neconectat la un grup) și site de comunicare.

>[!Important]
> Nu ștergeți site-ul rădăcină clasic pentru a crea un site de comunicare modern. Acest lucru nu este acceptat de Microsoft. Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizație inaccesibile pentru toți utilizatorii, până când restaurați site-ul sau creați un site nou la același URL. Vom comunica această caracteristică prin centrul de mesaje. Trebuie să vă așteptați ca caracteristica să fie activată în entitatea găzduită în scurt timp.

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu înlocuirea site-urilor
- Site-ul țintă poate returna o eroare "nu s-a găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie rescotocit pentru a actualiza indexul de căutare. Nu este necesar un pas manual aici, acesta va fi efectuat automat.
- Orice dependență de linkuri "statice" (cum ar fi sincronizarea fișierelor și fișierele OneNote) va trebui să fie corectată manual.
- Site-urile Project Server pot necesita validarea pentru a vă asigura că acestea sunt încă asociate corect. 
