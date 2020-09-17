---
title: Repararea fișierului. pst înainte de import
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799108"
---
# <a name="repair-pst-file-before-importing"></a>Repararea fișierului. pst înainte de import

Înainte de a importa un fișier. pst în Outlook, Verificați dacă fișierul nu este deteriorat prin repararea fișierului:

1. Ieșiți din Outlook.

2. Găsiți și rulează `Scanpst.exe` în folderul de programe Office (C:\Program Files (x86) \Microsoft Office\root\Office \<Version\> sau C:\Program Files\Microsoft Office\root\Office \<Version\> ).

3. În **Instrumentul de reparare Inbox din Microsoft Outlook**, faceți clic pe **Răsfoire** pentru a găsi fișierul. pst (de exemplu, în C:\Users \\<nume de utilizator \> \AppData\Local\Microsoft\Outlook). Selectați fișierul. pst, apoi faceți clic pe **Deschidere**.

4. Faceți clic pe **pornire** pentru a începe scanarea.

5. Dacă se găsesc erori în fișier, faceți clic pe **Reparare**, apoi faceți clic pe **OK** când repararea este finalizată.

6. Încercați să importați din nou fișierul. pst în Outlook.

Pentru mai multe informații, consultați [repararea fișierelor de date Outlook](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) și [remedierea problemelor cu importul unui fișier. pst Outlook](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
