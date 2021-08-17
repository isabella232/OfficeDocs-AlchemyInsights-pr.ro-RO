---
title: Remedierea politicii de conexiune
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314856"
---
# <a name="fix-connection-policy"></a>Remedierea politicii de conexiune

Mesajul de e-mail a fost marcat ca sigur și livrat în Inboxul utilizatorului, deoarece adresa IP sursă a fost marcată ca sigură în politica implicită de filtrare a conexiunii. Pentru a revizui politica, urmați acești pași:

1. În portalul de Microsoft 365 Defender de la , accesați Trimiterea prin e-& a politicilor de colaborare & regulilor de amenințare <https://security.microsoft.com/>  \>  \>  \> **antispam** **în secțiunea** Politici.

   Pentru a merge direct la **pagina Politici antispam,** utilizați <https://security.microsoft.com/antispam> .

2. Pe pagina **Politici antispam,** selectați politica denumită Politica de filtrare a conexiunii **(Implicit),** făcând clic pe numele politicii.

3. În meniul volant detalii care apare, faceți clic **pe Editați politica de filtrare** a conexiunii din **secțiunea Filtrare** conexiune.

4. Examinați intrările din **secțiunea Se permit întotdeauna mesajele** din următoarea secțiune de adrese IP sau intervale de adrese și vedeți dacă **s-a selectat Activați lista** sigură.

   **Notă:** Microsoft se abonează la surse terțe ale expeditorilor de încredere. Dacă este activată lista sigură, acești expeditori de încredere nu sunt marcați greșit ca spam. Vă recomandăm să selectați această opțiune, deoarece va reduce numărul de rezultate fals pozitive (mesaje de e-mail bune clasificate ca spam) pe care le primiți.

Pentru mai multe informații, consultați [Configurarea filtrării conexiunii.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
