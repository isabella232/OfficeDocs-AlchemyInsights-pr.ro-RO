---
title: 1065 Dezaprobarea intervalelor de adrese IP de ieșire EOPMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704609"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Dezaprobarea intervalelor de adrese IP de ieșire ale EOP

Am detectat o problemă potențială cu organizația dvs., care (dacă nu este corectată până la 26 octombrie 2018) ar putea întrerupe fluxul de corespondență către destinațiile locale sau externe. După s-a comunicat anterior, pentru a simplifica gestionarea intervalului de adrese IP, consolidăm intervalele de adrese IP Exchange Online Protection (EOP) care sunt utilizate pentru a trimite și primi e-mailuri în afara Microsoft 365. Analiza noastră indică faptul că una sau mai multe surse de e-mail externe sau destinații pe care le-ați configurat în conectorii fluxului de corespondență nu acceptă conexiuni din intervalele de adrese IP afișate [aici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Acționați înainte de 26 octombrie pentru a vă asigura că aceste surse și destinații vor accepta conexiuni la și de la toate [adresele IP EOP publicate](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Pentru mai multe informații despre această modificare, vă rugăm să consultați Mesaje Center posturi [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Notă:** Dacă ați utilizat anterior publicarea IP sau URL prin HTML, XML și RSS pentru actualizări de puncte finale, de asemenea, ar trebui să migreze la noile servicii web pentru automatizarea acestor tipuri de actualizări. Pentru mai multe informații, consultați [Categoriile de puncte finale Microsoft 365 și serviciul web Microsoft 365 IP Address and URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
