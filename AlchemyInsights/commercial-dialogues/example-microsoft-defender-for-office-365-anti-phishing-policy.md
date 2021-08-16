---
title: Exemplu de Microsoft Defender pentru Office 365 anti-phishing
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035018"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Exemplu de Microsoft Defender pentru Office 365 anti-phishing

Aceste setări activează o politică numită *Domeniu și CEO*. Această politică asigură atât protecția utilizatorilor, cât și a domeniului împotriva substituirii zonării, apoi aplică politica la toate mesajele de e-mail primite de utilizatorii din domeniu. Mai întâi, adăugați următoarele informații pentru a crea politica:

- **Nume:** Descriere domeniu și ceo: asigură că ceo și domeniul dvs. nu vor fi substituiți de identitate.
  **Se aplică la:** **Selectați Domeniul destinatarului este**. Sub **Oricare dintre acestea**, **selectați Alegeți**, apoi selectați un domeniu. Selectați **+ Adăugare**. Bifați caseta de selectare de lângă numele domeniului din listă (de exemplu, *nume contoso.com*), apoi selectați **Adăugare**. Selectați **Terminat**.
- După ce se creează politica, puteți să reglați fin politica utilizând următoarele opțiuni:
  - **Adăugați utilizatori pentru a proteja:** Pentru acest exemplu, adăugați adresa de e-mail a ceoului, cel puțin.
  - **Adăugați domenii pentru a proteja:** adăugați domeniul organizațional care include biroul de CEO.
  - **Alegeți acțiuni:** **Pentru** Dacă e-mailul este trimis de un utilizator cu identitate , selectați Redirecționare mesaj la altă adresă de e-mail **,** apoi introduceți adresa de e-mail a administratorului de securitate (de *exemplu, securityadmin@contoso.com*). Pentru Dacă **e-mailul este trimis de un domeniu cu substituire a zonei,** selectați **Puneți în carantină mesajul.**
  - **Informații despre cutia** poștală: Această opțiune este selectată în mod implicit atunci când creați o nouă politică anti-phishing. Lăsați această setare **La, pentru** rezultate optime.
  - **Adăugați expeditori și domenii de încredere:** Pentru acest exemplu, nu definiți înlocuiri.
- După ce ați revizuit setările, selectați Creați această **politică sau Salvați** **,** după cum este necesar.

Pentru a afla mai multe, [consultați Politicile anti-phishing din Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
