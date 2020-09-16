---
title: Liste mari SharePoint
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
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720145"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Lucrul cu liste și biblioteci mari în SharePoint

Listele și bibliotecile SharePoint pot conține până la 30.000.000 de elemente, dar atunci când au mai mult de 5.000 de elemente, este posibil să vedeți o eroare de prag a vizualizării listă atunci când încercați să lucrați cu ele. Acest prag există pentru a menține performanța serviciului. Acesta nu poate fi modificat. Pentru a evita atingerea acestui prag:

**Utilizați modern**

Vizualizările care afișează cele mai bune elemente funcționează cel mai bine în experiența modernă. [Utilizați experiența modernă](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) pentru a evita erorile pe care le-ați putea vedea în experiența clasică.

**Adăugarea indexurilor**

Atunci când filtrați sau sortați după o coloană care nu are un index, este posibil să vedeți un mesaj de eroare. [Adăugați manual un index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) din **Setări listă** din meniul Setări, apoi **coloane indexate**.

**Editarea vizualizării listă**

Dacă apare o eroare atunci când lucrați cu o listă mare, [editați vizualizarea listă](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Următoarele patru modificări vor elimina erorile de prag pentru vizualizarea listă. Efectuați toate cele patru modificări pentru a elimina toate erorile. Dacă primiți în continuare erori, verificați [gestionarea listelor și bibliotecilor mari](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Selectați **fără** din ambele **Sortare după coloană** , **apoi sortați după coloană**.
2. Selectați **fără** din **primul grup după coloană** , **apoi grupați după coloană**.
3. Selectați **fără** pentru toate coloanele din secțiunea **totaluri** .
4. Deselectați toate, dar o coloană pentru afișare din secțiunea **coloane** .

