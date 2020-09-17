---
title: 1065 dezaprobarea adresei IP de ieșire EOP rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806807"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Dezaprobarea zonelor de adrese IP de ieșire EOP

Am detectat o problemă potențială cu organizația dvs., care (dacă nu este corectată până la 26 octombrie 2018) poate întrerupe fluxul de corespondență la destinațiile locale sau externe. Așa cum s-a comunicat anterior, pentru a simplifica gestionarea intervalelor de adrese IP, sintetizăm intervalele de adrese IP Exchange Online Protection (EOP) care sunt utilizate pentru a trimite și a primi mesaje de e-mail în afara Microsoft 365. Analiza noastră indică faptul că una sau mai multe dintre sursele sau destinațiile externe de e-mail pe care le-ați configurat în conectorii fluxului de corespondență nu acceptă conexiuni din intervalele de adrese IP afișate [aici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Acționeze înainte de 26 octombrie pentru a vă asigura că aceste surse și destinații vor accepta conexiuni la și de la toate [adresele IP de EOP publicate](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Pentru mai multe informații despre această modificare, consultați postările din centrul de mesaje [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Notă**: dacă ați utilizat anterior publicarea IP sau URL prin intermediul actualizărilor HTML, XML și RSS pentru Endpoint, ar trebui, de asemenea, să migrați la noile servicii web pentru automatizarea acestor tipuri de actualizări. Pentru mai multe informații, consultați [microsoft 365 Endpoint categorii și microsoft 365 IP Address și URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
