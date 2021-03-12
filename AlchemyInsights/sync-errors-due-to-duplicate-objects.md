---
title: 902 (erorile de sincronizare din cauza obiectelor dublate)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708074"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erorile de sincronizare din cauza obiectelor dublate

Este posibil să primiți unul dintre următoarele mesaje de eroare atunci când se termină sincronizarea directorului în Microsoft 365:

- Nu se poate actualiza acest obiect în Microsoft Online Services, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din directorul local.

- Un obiect sincronizat cu aceeași adresă proxy există deja în directorul Microsoft Online Services.

- Nu se poate actualiza acest obiect, deoarece următoarele atribute asociate cu acest obiect au valori care pot fi deja asociate cu un alt obiect din serviciile directorului local: UserPrincipalName.

Pentru a identifica și a remedia problema, descărcați și derulează [Instrumentul de remediere a erorilor IdFix DirSync](https://github.com/Microsoft/idfix).

Pentru mai multe informații, consultați [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
