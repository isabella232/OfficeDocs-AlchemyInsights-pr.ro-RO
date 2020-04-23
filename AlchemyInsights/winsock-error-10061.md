---
title: 1554 Winsock eroare 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766181"
---
# <a name="winsock-error-10061"></a>Eroare Winsock 10061

Acest cod de eroare înseamnă că Microsoft nu a putut stabili un socket TCP (conexiune) cu gazda țintă. Cauza cea mai probabilă a acestei erori este o problemă cu configurația paravanului de protecție. Pentru a remedia problema, verificați aceste setări:

- Verificați configurația paravanului de protecție cu informațiile din [url-urile Microsoft 365 și intervalele de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Dacă eroarea este specifică Exchange Online Protection (EOP), ar fi trebuit să fi fost notificat anterior la o modificare a [adreselor IP Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verificați că furnizorul de servicii Internet (ISP) nu blochează portul.

- Verificați setările inteligente de gazdă și server țintă în conectori.

Rețineți că Microsoft 365 nu blochează *conexiunile primite* în acest mod.
