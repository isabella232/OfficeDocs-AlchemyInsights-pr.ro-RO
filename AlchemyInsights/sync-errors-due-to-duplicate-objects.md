---
title: 902 (Erori de sincronizare din cauza obiectelor dublate)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998806"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erori de sincronizare din cauza obiectelor dublate

Este posibil să primiți unul dintre următoarele mesaje de eroare atunci când sincronizarea directorului se termină în Microsoft 365:

- Nu se poate actualiza acest obiect în Microsoft Online Services, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din directorul local.

- Un obiect sincronizat cu aceeași adresă proxy există deja în directorul Microsoft Online Services.

- Nu se poate actualiza acest obiect, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din serviciile dvs. locale de director: UserPrincipalName.

Pentru a identifica și a remedia problema, descărcați și rulați Instrumentul de remediere [a erorilor IdFix DirSync.](https://github.com/Microsoft/idfix)

Pentru mai multe informații, [consultați KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
