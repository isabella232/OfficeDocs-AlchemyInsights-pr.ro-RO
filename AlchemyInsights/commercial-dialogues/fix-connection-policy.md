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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888418"
---
# <a name="fix-connection-policy"></a>Remedierea politicii de conexiune

Mesajul de e-mail a fost marcat ca sigur și livrat în Inboxul utilizatorului, deoarece adresa IP sursă a fost marcată ca sigură în politica implicită de filtrare a conexiunii. Pentru a revizui politica, urmați acești pași:

1. În portalul de Microsoft 365 Defender de la , accesați Trimiterea prin e-mail & politicilor de colaborare & Reguli <https://security.microsoft.com/>  \>  \>  \> **antispam** în **secțiunea** Politici.

   Pentru a merge direct la **pagina Politici antispam,** utilizați <https://security.microsoft.com/antispam> .

2. Pe pagina **Politici antispam,** selectați politica denumită Politica de filtrare a conexiunii **(Implicit),** făcând clic pe numele politicii.

3. În meniul volant detalii care apare, faceți clic **pe Editați politica de filtrare** a conexiunii din **secțiunea Filtrare** conexiune.

4. Examinați intrările din **secțiunea Se permit întotdeauna mesajele** din următoarea secțiune de adrese IP sau intervale de adrese și vedeți dacă **s-a selectat Activați lista** sigură.

   > [!NOTE]
   > Microsoft se abonează la surse terțe ale expeditorilor de încredere. Dacă este activată lista sigură, acești expeditori de încredere nu sunt marcați greșit ca spam. Vă recomandăm să selectați această opțiune, deoarece va reduce numărul de rezultate fals pozitive (mesaje de e-mail bune clasificate ca spam) pe care le primiți.

Pentru mai multe informații, consultați [Configurarea filtrării conexiunii.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
