---
title: Depanarea problemelor de instalare MDATP pe un Mac
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091068"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Depanarea problemelor de instalare MDATP pe un Mac

Dacă instalarea manuală nu **reușește, pagina** Rezumat a expertului de instalare afișează următoarea eroare:

"A apărut o eroare în timpul instalării. Programul de instalare a întâmpinat o eroare care a determinat ca instalarea să nu reușească. Contactați producătorul software-ului pentru asistență."

Pentru implementările MDM, pagina afișează, de asemenea, o eroare generică de instalare.

Deși nu afișăm erorile exacte pentru utilizatorii finali, păstrăm un fișier jurnal cu progresul instalării, în **/Library/Logs/Microsoft/mdatp/install.log.** Fiecare sesiune de instalare se adaugă la acest fișier jurnal. Pentru a rezultatele ultimei sesiuni de instalare, utilizați `sed` .

Pentru a afla mai multe, [consultați Depanarea problemelor de instalare pentru Microsoft Defender ATP pentru Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
