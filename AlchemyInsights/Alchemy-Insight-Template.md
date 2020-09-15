---
title: la fel ca numele de fișier este cel mai bun
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664146"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Antetul Alchemy necesar H1, H2 servește nu funcționează."
Cele mai bune practici și instrucțiuni pentru crearea Alchemy:

1. Nu **imbricați Insights Alchemy în foldere**-aceasta va întrerupe structura URL-ului. Încercăm să reparăm asta.
1. Fișierele din folderul **AlchemyInsights** trebuie să aibă nume de fișiere minuscule cu cratime pentru spațiile ex. ***cum să activați-litigii-țineți***.
    1. Includeți ID-ul de regulă sau ID-ul de cupă din [portalul partener Alchemy](https://alchemyportal.azurewebsites.net) în câmpul MS. Custom. exemplu. ***MS. Custom: 100021***
1. Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.
1. În [portalul partener Alchemy](https://alchemyportal.azurewebsites.net), navigați în jos la secțiunea **Customer Insight title:** și utilizați-o ca punct de pornire pentru titlul H1 pentru înțelegere. 
    > [!NOTE]
    > Insights Alchemy trebuie să aibă doar un singur H1 în partea de sus sau se vor rupe în producție. H2s nu redă niciuna dintre **bold** aceste convenții pentru a semnifica secțiuni separate.
1. Apoi, completați corpul de text utilizând schița de material din secțiunea Customer Insights a paginii de reguli Alchemy
    1. Listele cu marcatori sunt în regulă
    1. Și liste numerotate
    1. **Aldin** și *cursiv* sunt a-OK
    1. Linkurile trebuie să fie întotdeauna **"linkuri către web"/external** sau **Deep-linkuri către elemente de interfață utilizator**, nu către Linkuri interne.
    1. Imaginile nu sunt acceptate oficial în acest moment, dar se află în foaia de parcurs.

Iar acest lucru este într-adevăr deja un pic prea lung. Cea mai bună practică este de aproximativ 400 de caractere---------------------------------

După ce conținutul este gata, trageți-l la ramura în direct. Apoi, accesați portalul pentru [parteneri Alchemy](https://alchemyportal.azurewebsites.net) și introduceți numele de fișier în câmpul URL. 