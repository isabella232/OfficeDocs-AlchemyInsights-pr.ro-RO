---
title: Site modern drept site rădăcină
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327614"
---
# <a name="modern-site-as-root-site"></a>Site modern ca site rădăcină

Am început să lamurim o caracteristică nouă care vă va permite să schimbați site-ul rădăcină clasic [al site-ului cu un site modern.](https://docs.microsoft.com/sharepoint/modern-root-site) Utilizați [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) pentru a transfera locația unui site cu un alt site în timp ce arhivați site-ul original. Disponibil atât pentru site-ul de echipă (neconectat la un grup), cât și pentru Site-ul de comunicare.

**Important:** Nu ștergeți site-ul rădăcină clasic pentru a crea un site de comunicare modern. Acest lucru nu este acceptat de Microsoft. Ștergerea site-ului rădăcină va face toate site-urile SharePoint din organizație inaccesibile pentru toți utilizatorii, până când restaurați site-ul sau creați un site nou la același URL. Vom comunica această caracteristică prin intermediul centrului de mesaje. Ar trebui să vă așteptați ca această caracteristică să fie activată în entitatea găzduită în scurt timp.

## <a name="known-issues-with-swapping-sites"></a>Probleme cunoscute cu comutarea între site-uri
- Site-ul țintă poate returna o eroare "nu a fost găsit" (HTTP 404) pentru o perioadă scurtă de timp.
- Conținutul va trebui să fie resuficat pentru a actualiza indexul de căutare. Nu este necesar niciun pas manual aici. Acest lucru va fi efectuat automat.
- Orice legătură dependentă de linkurile "statice" (cum ar fi Sincronizare fișier OneNote fișiere) va trebui corectată manual.
- Project Site-urile server pot avea nevoie să fie validate, pentru a vă asigura că sunt în continuare asociate corect. 
