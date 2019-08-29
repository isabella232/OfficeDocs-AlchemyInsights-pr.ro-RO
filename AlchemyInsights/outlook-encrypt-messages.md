---
title: S/MIME în Outlook pe web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666852"
---
# <a name="encrypt-email-messages-in-outlook"></a>Criptaţi mesajele de e-mail în Outlook

Criptare de mesaj Office 365 este construit pe Microsoft Azure administrarea drepturilor (RMS azuriu), care face parte din protecția informațiilor cu Azure. În cazul în care abonamentul include Azure Rights Management sau protecția informațiilor Azure, **nu aveţi nevoie să ia orice măsuri pentru a activa manual sau activa** şi serviciul de gestionare a drepturilor.

Bazat pe feedback-ul clientului, ne va nu mai fi care să permită Exchange mail fluxul reguli să cripteze automat outbound e-mail care conţine anumit tip de informaţii sensibile în chiriaşul dumneavoastră în mod implicit. În schimb, ne oferă instrucţiuni detaliate pe cum pot face acest lucru singuri. Pentru detalii suplimentare despre cum să creaţi o regulă de transport pentru a cripta datele sensibile, a se vedea [acest articol](https://aka.ms/OmeEtr).

- Dacă utilizaţi Outlook pe Web (fostă **OWA**): atunci când compuneţi un mesaj de poştă electronică, faceţi clic pe **Protejare** în OWA. Aceasta se va aplica "Face nu transmite" permisiunea. Faceţi clic pe **Schimbare permisiuni** şi selectaţi **criptare** pentru a cripta doar mesajul.

- În cazul în care folosind **clientul Outlook**: pentru a expedia un mesaj criptat din Outlook 2013 sau 2016 sau Outlook 2016 pentru Mac, selectaţi **Opţiuni** > **permisiunile**, apoi selectaţi opţiunea de protecţie ce trebuie.

- Să **cripteze automat toate e-mail** trimise unor destinatari sau organizaţiile partenere externe, trebuie să creaţi o regulă de transport a fluxului de corespondenţă în centrul de administrare Exchange. Instrucţiuni detaliate sunt oferite în [acest articol de sprijin](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

