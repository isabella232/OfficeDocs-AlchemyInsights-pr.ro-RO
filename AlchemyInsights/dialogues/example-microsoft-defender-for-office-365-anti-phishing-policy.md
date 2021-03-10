---
title: Exemplu de politică anti-phishing Microsoft Defender pentru Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695644"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exemplu de politică anti-phishing Microsoft Defender pentru Office 365

Aceste setări permit o politică denumită *Domain și CEO*. Această politică oferă protecție pentru utilizator și domeniu de la personificare, apoi aplică politica pentru toate mesajele de e-mail primite de utilizatorii din domeniu. Mai întâi, adăugați următoarele informații pentru a crea politica:

- **Nume**: Domain and CEO **Description**: asigură faptul că directorul general și domeniul dumneavoastră nu sunt imitate.
  **Aplicată la**: selectați **domeniul destinatarului este**. Sub **oricare dintre acestea**, selectați **alegere**, apoi selectați un domeniu. Selectați **+ Adăugare**. Bifați caseta de selectare de lângă numele domeniului din listă (de exemplu, *contoso.com*), apoi selectați **Adăugare**. Selectați **gata**.
- După ce se creează politica, puteți ajusta politica utilizând următoarele opțiuni:
  - **Adăugați utilizatori pentru a proteja:** Pentru acest exemplu, adăugați adresa de e-mail a CEO-ului, cel puțin.
  - **Adăugați domenii de protejat**: adăugați domeniul organizațional care include Office pentru CEO.
  - **Alegeți acțiuni**: pentru **dacă e-mailul este trimis de un utilizator pretins**, selectați **redirecționați mesajul către altă adresă de e-mail**, apoi introduceți adresa de e-mail a administratorului de securitate (de exemplu, *securityadmin@contoso.com*). **Dacă e-mailul este trimis de un domeniu pretins**, selectați **carantină mesaj**.
  - **Serviciul de informații pentru cutia poștală**: în mod implicit, această opțiune este selectată atunci când creați o nouă politică anti-phishing. Lăsați această setare **la** cele mai bune rezultate.
  - **Adăugați expeditori și domenii de încredere:** Pentru acest exemplu, nu definiți nicio suprascrie.
- După ce ați revizuit setările, selectați **Creați această politică** sau **Salvați**, după cum este cazul.

Pentru a afla mai multe, consultați [politici anti-phishing în Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
