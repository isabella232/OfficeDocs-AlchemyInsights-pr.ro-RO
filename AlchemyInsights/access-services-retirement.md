---
title: Accesarea retragerea serviciilor
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938707"
---
# <a name="access-services-retirement"></a>Accesarea retragerea serviciilor

Așa cum am anunțat inițial în MC97576, în martie 2017 și a continuă să comunicăm anul trecut până când Access Services vor fi retrase. Următoarea fază din acest proces va fi eliminarea bazelor de date web Access care utilizează o SharePoint ca stocare a datelor subiacentă.

**Cum mă afectează acest lucru?**

Începând din iunie 2019, vom opri crearea de noi baze de date Access în SharePoint Online și vom închide serviciul și toate aplicațiile rămase până în aprilie 2020.

**Ce trebuie să fac pentru a mă pregăti pentru această modificare?**

Vă recomandăm să creați un plan de tranziție pentru bazele de date web Access ale organizației dvs. Administratorii pot utiliza [scanerul SharePoint Access pentru](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) a obține un inventar al aplicațiilor Access pe care le utilizează site-urile.

Există mai multe modalități de a migra datele bazelor de date web Access:

- Importul într-o bază de date Access locală (. ACCDB) sau într-un Excel date.
- De asemenea, vă recomandăm să explorați Microsoft PowerApps ca platformă alternativă pentru a crea soluții de business fără cod pentru web și dispozitive mobile.