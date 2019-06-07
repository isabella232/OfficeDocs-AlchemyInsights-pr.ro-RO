---
title: 1065 dezaprobare EOP outbound IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752967"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Dezaprobare de EOP ieşire variază de adresa IP

Ne-am detectat o problemă potenţială cu organizaţiei (dacă nu este corectată de 26 octombrie 2018) s-ar putea rupe fluxul de corespondenţă de la local sau destinaţii externe. Ca anterior comunicate, pentru a simplifica gestionarea gama IP adresa, am centralizaţi Exchange Online protecţia (EOP) IP adresa intervalele care sunt folosite pentru a trimite şi primi poştă electronică în afara de Office 365. Analiza noastră indică faptul că una sau mai multe de e-mail extern surse sau destinaţii care aţi configurat în conectorii de fluxul de corespondenţă nu sunt accepta conexiuni de la IP adresă intervalele afişate [aici](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Acţionează înainte de 26 octombrie, pentru a asigura aceste surse şi destinaţii va accepta conexiuni la şi de la toate [adresele EOP IP a publicat](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Pentru mai multe informaţii despre această schimbare, vă rugăm să consultaţi Centrul de mesaje posturi [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)sau [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Notă**: dacă aţi utilizat anterior publicarii IP sau URL-ul prin intermediul HTML, XML şi RSS pentru actualizări de final, de asemenea, ar trebui să migra la noile servicii web pentru automatizarea acestor tipuri de actualizări. Pentru mai multe informaţii, a se vedea [categoriile de endpoint Office 365 si Office 365 adresa IP şi URL serviciu web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
