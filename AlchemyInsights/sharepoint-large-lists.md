---
title: SharePoint liste mari
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941620"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Lucrul cu liste și biblioteci mari în SharePoint

SharePoint listele și bibliotecile pot conține până la 30 de milioane de elemente, dar atunci când au mai mult de 5.000 de elemente, este posibil să vedeți o eroare de Prag vizualizare listă atunci când încercați să lucrați cu ele. Acest prag există pentru a menține performanța serviciului. Acesta nu poate fi modificat. Pentru a evita să atingeți acest prag:

**Utilizați un design modern**

Vizualizări care afișează mai multe elemente funcționează cel mai bine în experiența modernă. [Utilizați experiența modernă pentru a](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) evita erorile pe care este posibil să le vedeți în experiența clasică.

**Adăugarea de indexuri**

Când filtrați sau sortați după o coloană care nu are index, este posibil să vedeți un mesaj de eroare. [Adăugați manual un index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) din **lista de Setări** din meniul setări, apoi **Coloane indexate.**

**Editarea vizualizării listă**

Dacă apare o eroare atunci când lucrați cu o listă mare, [editați vizualizarea listă.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)

Următoarele patru modificări vor elimina erorile prag vizualizare listă. Efectuați toate cele patru modificări pentru a elimina toate erorile. Dacă încă se primesc erori, consultați Gestionarea [listelor și bibliotecilor mari.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)

1. Selectați **Fără** din Sortare **mai întâi după coloană** **și Apoi sortați după coloană.**
2. Selectați Fără atât **Grupare mai întâi după coloană,** **apoi grupare după coloană.** 
3. **Selectați** Fără pentru toate coloanele din **secțiunea Totaluri.**
4. Deselectați toate coloanele, cu o singură coloană pentru afișare, **din secțiunea** Coloane.

