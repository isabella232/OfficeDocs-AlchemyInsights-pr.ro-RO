---
title: Site-ul modernă ca site-ul rădăcină
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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543865"
---
# <a name="modern-site-as-root-site"></a>Site-ul modernă ca site-ul rădăcină

Am început să rollout o caracteristică nouă care vă va permite să vă site-ul clasic site-ul rădăcină, cu un site modern de swap. Utilizaţi [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a schimba locaţia de un site cu un alt site în timp ce site-ul original de arhivare. Disponibil pentru echipa site-ului (nu este conectat la un grup) şi de site-ul de comunicare. 

>[!Important]
> Imposibil de șters site-ul clasic rădăcină pentru a crea un Site de comunicare moderne. Acest lucru nu este acceptată de Microsoft. Ştergerea site-ul rădăcină va face toate site-urile SharePoint din organizaţie inaccesibile pentru toţi utilizatorii, până la restaurarea site-ul sau de a crea un site nou la aceeaşi adresă URL. Ne veţi fi comunicarea această caracteristică prin centrul de mesaje. Ar trebui să aşteptaţi caracteristică să fie pornit în chiriaşul dumneavoastră la scurt timp.

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu schimbarea site-uri
- Site-ul ţintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie el scotocit din nou pentru a actualiza indexul de căutare. Nu există nici un manual pas necesar aici, acest lucru se va face automat.
- Nimic depinde şi de link-uri "statice" (cum ar fi fişiere fişier sincronizare și OneNote) va trebui să manual corectate.
- Proiect Server site-uri trebuie să fie validate pentru a se asigura că acestea sunt încă asociate corect. 
