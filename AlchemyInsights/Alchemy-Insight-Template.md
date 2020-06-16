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
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750982"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Obligatoriu Alchemy Header H1, H2 nu funcționează."
Cele mai bune practici și orientări pentru alchimie autor:

1. **Nu cuib Alchemy Insights în foldere**- acest lucru va rupe structura URL-ul. Căutăm să reparăm asta.
1. Fișierele din folderul **AlchemyInsights** ar trebui să aibă nume de fișiere minuscule cu cratime pentru spațiiex. ***cum să-enable-litigation-hold***.
    1. Includeți ID-ul de regulă sau ID-ul de găleată din [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net) în câmpul ms.custom. Ex. ***ms.custom: 100021***
1. Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.
1. În [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net), navigați în jos la secțiunea **Customer Insight Title:** și utilizați-o ca punct de plecare pentru titlul H1 pentru înțelegere. 
    > [!NOTE]
    > Alchemy Insights trebuie să aibă doar un singur H1 în partea de sus sau se va rupe în producție. H2-urile nu redau nici așa că utilizați convenții **aldine** sau alte convenții pentru a semnifica secțiuni separate.
1. Apoi, completați textul corpului utilizând materialul schiță din secțiunea Customer Insights a paginii Alchemy Rule
    1. Listele cu marcatori sunt în regulă
    1. Liste numerotate prea
    1. **Bold** și *cursiv* sunt a-ok
    1. Link-uri ar trebui să fie întotdeauna fie **"link-uri către web"/extern** sau **deep-link-uri către elemente ui, nu link-uri**interne.
    1. Imaginile nu sunt acceptate oficial în acest moment, dar este pe foaia de parcurs.

Și asta e deja un pic prea lung. Cele mai bune practici este de aproximativ 400 de caractere ---------------------------------

Odată ce conținutul este gata, trageți-l la ramura live. Apoi, accesați [portalul Alchemy Partner](https://alchemyportal.azurewebsites.net) și introduceți numele fișierului în câmpul URL. 