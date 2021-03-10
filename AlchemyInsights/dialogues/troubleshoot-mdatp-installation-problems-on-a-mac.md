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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696093"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Depanarea problemelor de instalare MDATP pe un Mac

Dacă instalarea manuală nu reușește, pagina **Rezumat** a expertului de instalare afișează următoarea eroare:

"A apărut o eroare în timpul instalării. Programul de instalare a întâlnit o eroare care a determinat instalarea să nu reușească. Contactați producătorul software-ului pentru asistență. "

Pentru implementările MDM, pagina afișează și o eroare generică de instalare.

Deși nu se afișează erorile exacte pentru utilizatorii finali, păstrăm un fișier jurnal cu progresul instalării, în **/Library/logs/Microsoft/mdatp/install.log**. Fiecare sesiune de instalare se adaugă la acest fișier jurnal. Pentru a afișa numai ultima sesiune de instalare, utilizați `sed` .

Pentru a afla mai multe, consultați [Depanarea problemelor de instalare pentru Microsoft Defender ATP pentru Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
