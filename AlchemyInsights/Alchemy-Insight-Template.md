---
title: la fel ca numele de fișier este cel mai bun
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676545"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Obligatoriu Alchimie Antet H1, H2 nu funcționează.
Cele mai bune practici și orientări pentru alchimie autor:

1. **Nu cuib Alchimie Insights în foldere**- acest lucru se va rupe structura URL-ul. Căutăm să reparăm asta.
1. Fișierele din folderul **AlchemyInsights** ar trebui să aibă nume de fișiere cu litere mici cu cratime pentru spații ex. ***cum să-enable-litigii-hold***.
    1. Includeți ID-ul regulii sau ID-ul de găleată din [portalul Partener alchimie](https://alchemyportal.azurewebsites.net) din câmpul ms.custom. Ex. ***ms.custom: 100021 ms.custom: 100021 ms.custom: 100021***
1. Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.
1. În [portalul Partener alchimie,](https://alchemyportal.azurewebsites.net)navigați în jos la secțiunea **Titlu Customer Insight:** și utilizați-l ca punct de plecare pentru titlul H1 pentru înțelegere. 
    > [!NOTE]
    > Alchimie Insights trebuie să aibă doar un singur H1 în partea de sus sau se vor rupe în producție. H2-urile nu fac nici măcar alte **convenții,** nici alte convenții pentru a semnifica secțiuni separate.
1. Apoi, completați corpul text utilizând proiectul de material din secțiunea Statistici client din pagina Regula alchimiei
    1. Listele cu marcatori sunt în regulă.
    1. Liste numerotate prea
    1. **Îndrăzneț** și *cursiv* sunt a-ok
    1. Link-uri ar trebui să fie întotdeauna fie **"link-uri către web"/externe** sau **deep-link-uri către elemente UI,** nu link-uri interne.
    1. Imaginile nu sunt acceptate oficial în acest moment, dar sunt pe foaia de parcurs.

Și acest lucru este într-adevăr deja un pic prea mult timp. Cele mai bune practici sunt de aproximativ 400 de caractere ---------------------------------

Odată ce conținutul este gata, trageți-l la ramura live. Apoi, accesați [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net) și introduceți numele fișierului în câmpul URL. 