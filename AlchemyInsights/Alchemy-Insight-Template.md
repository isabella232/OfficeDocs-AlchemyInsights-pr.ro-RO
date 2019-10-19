---
title: fel ca filename este cel mai bun
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800057"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Necesar header Alchemy H1, H2's nu funcționează.
Cele mai bune practici și orientări pentru Authoring Alchemy:

1. Nu **cuib Alchemy Insights în dosare**-acest lucru va rupe structura URL-ul. Încercăm să reparăm asta.
1. Fișierele din folderul **Alchemyinsights** ar trebui să aibă nume de fișiere minuscule cu cratime pentru spațiile ex. ***să-Enable-litigiu-Hold***.
    1. Includeți ID-ul de regulă sau ID-ul Cupei din [portalul de parteneri alchimie](https://alchemyportal.azurewebsites.net) în câmpul MS. Custom. Ex. ***MS. Custom: 100021***
1. Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.
1. În [portalul pentru parteneri alchimie](https://alchemyportal.azurewebsites.net), navigați în jos la secțiunea **client Insight title:** și utilizați-o ca punct de plecare pentru titlul H1 pentru înțelegere. 
    > [!NOTE]
    > Alchemy Insights trebuie să aibă doar un singur H1 în partea de sus sau vor sparge în producție. H2s nu face nici atât utilizarea **Bold** sau alte convenții pentru a semnifica secțiuni separate.
1. Apoi, completați textul corpului utilizând proiectul de material din secțiunea statistici client din pagina de regulă alchimie
    1. Listele cu marcatori sunt bune
    1. Liste numerotate prea
    1. **Bold** și *cursiv* sunt un-OK
    1. Link-uri ar trebui să fie întotdeauna fie **"link-uri către web"/externe** sau **Deep-link-uri către elemente UI**, nu link-uri interne.
    1. Imaginile nu sunt acceptate oficial în acest moment, dar este pe foaia de parcurs.

Și acest lucru este într-adevăr deja un pic prea mult timp. Cele mai bune practici este de aproximativ 400 de caractere---------------------------------

După ce conținutul este gata, trageți-l în ramura live. Apoi, mergeți la [portalul de parteneri alchimie](https://alchemyportal.azurewebsites.net) și introduceți numele fișierului în câmpul URL. 