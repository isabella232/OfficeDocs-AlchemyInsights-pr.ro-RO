---
title: Servicii de acces de pensionare
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687270"
---
# <a name="access-services-retirement"></a>Servicii de acces de pensionare

Așa am anunțat inițial în MC97576, în martie 2017, și am continuat să comunicăm în ultimul an, Access Services sunt retrase. Următoarea fază în acest proces va fi eliminarea bazelor de date Web Access care utilizează liste SharePoint ca stocare de date subiacente.

**mă afectează asta?**

Începând cu luna iunie 2019, vom opri crearea de noi baze de date Access în SharePoint Online și vom închide serviciul și toate aplicațiile rămase până în aprilie 2020.

**Ce trebuie să fac pentru a mă pregăti pentru această schimbare?**

Vă încurajăm să creați un plan de tranziție pentru bazele de date web Access ale organizației dvs. Administratorii pot utiliza [scanerul de aplicații SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pentru a obține un inventar al aplicațiilor Access pe care le utilizează site-urile.

Există mai multe moduri de migrare a datelor bazelor de date web Access:

- Importul într-o bază de date Access locală (. ACCDB) sau într-un fișier Excel.
- De asemenea, vă recomandăm să explorați Microsoft PowerApps ca o platformă alternativă pentru a crea soluții de afaceri fără cod pentru dispozitive web și mobile.