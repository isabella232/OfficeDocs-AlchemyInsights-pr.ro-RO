---
title: Servicii de acces la pensie
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747796"
---
# <a name="access-services-retirement"></a>Servicii de acces la pensie

Așa am anunțat inițial în MC97576, în martie 2017, și a continuat să comunice pe parcursul anului trecut servicii de acces sunt fiind retras din Office 365. Următoarea fază din acest proces va fi eliminarea bazelor de date Access web care utilizează liste SharePoint ca stocarea datelor subiacente.

**mă afectează asta?**

Începând cu iunie 2019, vom opri crearea de noi baze de date Access în SharePoint Online și închideți serviciul și orice aplicații rămase până în aprilie 2020.

**Ce trebuie să fac pentru a mă pregăti pentru această schimbare?**

Vă încurajăm să creați un plan de tranziție pentru bazele de date Web Access ale organizației dvs. Administratorii pot utiliza [scanerul aplicației SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pentru a obține un inventar al aplicațiilor Access pe care le utilizează site-urile.

Există mai multe modalități de a migra datele de baze de date Web Access:

- Importul într-o bază de date Access locală (. ACCDB) sau într-un fișier Excel.
- De asemenea, recomandăm explorarea Microsoft PowerApps ca o platformă alternativă pentru a crea soluții de afaceri fără cod pentru dispozitive web și mobile.