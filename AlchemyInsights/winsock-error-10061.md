---
title: 1554 Winsock eroare 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698874"
---
# <a name="winsock-error-10061"></a>Eroare Winsock 10061

Acest cod de eroare înseamnă că Microsoft nu a putut stabili un socket TCP (o conexiune) cu gazda țintă. Cauza cea mai probabilă a acestei erori este o problemă cu Configurarea paravanului de protecție. Pentru a remedia problema, Verificați aceste setări:

- Verificați configurația paravanului de protecție cu informațiile din [Microsoft 365 URL-uri și intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Dacă eroarea este specifică pentru Exchange Online Protection (EOP), ar fi trebuit să fiți notificat anterior unei modificări la [adresele IP Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verificați dacă furnizorul de servicii Internet (ISP) nu blochează portul.

- Verificați setările Smart Host și server țintă din conectori.

Rețineți că Microsoft 365 nu blochează conexiunile de *intrare* în acest mod.
