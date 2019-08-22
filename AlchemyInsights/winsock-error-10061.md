---
title: 1554 eroare Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530815"
---
# <a name="winsock-error-10061"></a>Eroare Winsock 10061

Acest cod de eroare înseamnă că Office 365 nu a putut stabili un socket TCP (conexiune) cu ţintă gazdă. Cel mai probabil cauza acestei erori este o problemă cu configuraţia paravanului de protecţie. Pentru a remedia problema, verificaţi aceste setări:

- Verificaţi configuraţia paravanului de protecţie cu informaţii la [Office 365 URL-uri şi intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- În cazul în care eroarea este specific pentru Exchange Online protecţia (EOP), tu ar trebui să au fost anterior notificate la o schimbare la [adresele IP de protecţie Online Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verificaţi că dumneavoastră Internet Service Provider (ISP) nu este blocarea portului.

- Verifica smart setările serverului de gazdă şi ţintă, în dumneavoastră conectori.

Reţineţi că Biroul 365 nu bloca conexiunile de *intrare* în acest mod.
