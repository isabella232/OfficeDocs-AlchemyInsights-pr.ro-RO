---
title: same as filename is best
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
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918907"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Antet Alchemy obligatoriu H1, H2 nu funcționează."
Cele mai bune practici și îndrumări pentru autor alchemy:

1. **Nu imbricați Alchemy Insights foldere**- aceasta va întreruperea structura URL-ului. Căutăm să remediam acest lucru.
1. Fișierele din folderul **AlchemyInsights trebuie** să aibă nume de fișiere mici cu cratime pentru spații, de exemplu. **_how-to-enable-litigation-hold_**.
    1. Includeți ID-ul regulii sau ID-ul [de bucket din portalul Partener Alchemy](https://alchemyportal.azurewebsites.net) în câmpul ms.custom. de ex. ***ms.custom: 100021***
1. Utilizați restul metadatelor din partea de sus a acestui fișier ca șablon.
1. În portalul [Partener Alchemy,](https://alchemyportal.azurewebsites.net)navigați în jos la secțiunea Titlu detaliu **client:** și utilizați-l ca punct de pornire pentru titlul H1 pentru detalii. 
    > [!NOTE]
    > Alchemy Insights MUST să aibă doar un singur H1 în partea de sus, altfel acestea se vor întrerupere în producție. H2 nu redă așadar utilizați convenții **aldine sau** de alt fel pentru a semna secțiuni separate.
1. În continuare, completați corpul de text utilizând materialul schiță din secțiunea Customer Insights a paginii Regulă Alchemy
    1. Listele cu marcatori sunt în regulă
    1. Și liste numerotate
    1. **Aldin** *și cursiv* sunt de-ok
    1. Linkurile trebuie să fie întotdeauna **"linkuri la web"/linkuri** de adâncime OR externe la **elementele de interfața de utilizator,** nu linkuri interne.
    1. Imaginile nu sunt acceptate oficial în acest moment, dar se află pe foaia de parcurs.

Și acest lucru este deja prea lung. Se pot exersa aproximativ 400 de caractere ---------------------------------

După ce conținutul este gata, trageți-l în ramura live. Apoi, accesați portalul [Partener Alchemy și](https://alchemyportal.azurewebsites.net) introduceți numele fișierului în câmpul URL. 