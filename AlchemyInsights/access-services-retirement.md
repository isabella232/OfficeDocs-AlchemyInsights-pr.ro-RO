---
title: Retragere servicii Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698694"
---
# <a name="access-services-retirement"></a>Retragere servicii Access

Așa cum am anunțat inițial în MC97576, în martie 2017, și am continuat să comunicăm în ultimul an Access Services sunt retrase. Următoarea etapă a acestui proces va fi eliminarea bazelor de date Web Access care utilizează liste SharePoint ca stocare de date subiacente.

**Cum mă afectează aceasta?**

Începând cu luna iunie 2019, vom opri crearea de noi baze de date Access în SharePoint Online și vom închide serviciul și toate aplicațiile rămase până în aprilie 2020.

**Ce trebuie să fac pentru a mă pregăti pentru această modificare?**

Vă recomandăm să creați un plan de tranziție pentru bazele de date Web Access ale organizației dvs. Administratorii pot utiliza [scanerul aplicației SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pentru a obține un inventar al aplicațiilor Access pe care le utilizează site-urile.

Există mai multe modalități de a migra datele din bazele de date Web Access:

- Importul într-o bază de date Access locală (. ACCDB) sau într-un fișier Excel.
- De asemenea, recomandăm explorarea Microsoft PowerApps ca platformă alternativă pentru a crea soluții de Business fără cod pentru dispozitive web și mobile.