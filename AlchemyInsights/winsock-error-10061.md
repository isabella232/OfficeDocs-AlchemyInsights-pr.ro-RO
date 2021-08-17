---
title: Eroare 1554Csei 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083242"
---
# <a name="winsock-error-10061"></a>Eroarea 10061 Dineu

Acest cod de eroare înseamnă că Microsoft nu a putut stabili un socket TCP (conexiune) cu gazda țintă. Cauza cea mai probabilă a acestei erori este o problemă cu configurarea firewallului. Pentru a remedia problema, verificați aceste setări:

- Verificați configurația firewallului cu informațiile [din Microsoft 365 URL-uri și intervale de adrese IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Dacă eroarea este specifică pentru Protecție Exchange Online (EOP), trebuie să fi fost notificat anterior cu o modificare a [adreselor IP Protecție Exchange Online ip.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Verificați dacă furnizorul dvs. de servicii internet (ISP) nu blochează portul.

- Verificați setările de gazdă inteligentă și server țintă din conectori.

Rețineți Microsoft 365 nu blochează *conexiunile de intrare* în acest mod.
