---
title: 1065 Perimarea zonelor de adrese IP de ieșire EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031274"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Perimarea intervalelor de adrese IP de ieșire EOP

Am detectat o problemă potențială cu organizația dvs., care (dacă nu este corectată de pe 26 octombrie 2018) poate eșua fluxul de corespondență către destinațiile dvs. externe sau local. După cum am comunicat anterior, pentru a simplifica gestionarea intervalelor de adrese IP, unim intervalele de adrese IP Protecție Exchange Online (EOP) care sunt utilizate pentru a trimite și a primi mesaje de e-mail în Microsoft 365. Analiza noastră indică faptul că una sau mai multe dintre sursele de e-mail externe sau destinațiile pe care le-ați configurat în conectorii de flux de corespondență nu acceptă conexiuni din intervalele de adrese IP afișate [aici.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Acționați înainte de 26 octombrie pentru a vă asigura că aceste surse și destinații vor accepta conexiuni la și de la [toate adresele IP EOP publicate.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Pentru mai multe informații despre această modificare, consultați Postările din Centrul de mesaje [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Notă:** Dacă ați utilizat anterior publicarea de IP sau URL prin HTML, XML și RSS pentru actualizări de puncte finale, ar trebui, de asemenea, să migrați la noile servicii web pentru automatizarea acestor tipuri de actualizări. Pentru mai multe informații, [consultați categoriile Microsoft 365 puncte finale și serviciul web Microsoft 365 IP și URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
