---
title: Trecerea de la serverele de nume Microsoft înapoi la gestionarea propriilor înregistrări DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506970"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Trecerea de la serverele de nume Microsoft înapoi la gestionarea propriilor înregistrări DNS

Ați modificat anterior înregistrările NS pentru a indicați spre Microsoft (ns1.bdm.microsoftonline.com), dar ați decis acum să vă gestionați propriile înregistrări DNS:

Pe site-ul web al registratorului de domeniu, schimbați serverul de nume înapoi la registratorul dvs. sau la setarea anterioară. Dacă nu vă familiarizați cu DNS, contactați asistența la registratorul de domeniu. Rețineți că propagarea modificărilor serverelor de nume poate dura până la 48 de ore. 

1. În portalul Microsoft 365, accesați Domenii **Setări**, bifați caseta de selectare de lângă domeniu  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)și selectați **Gestionare DNS**. 

2. În expert, selectați **Adăugați propriile înregistrări DNS și** finalizați expertul. Aceasta modifică modul de gestionare a DNS, apoi vă permite să adăugați înregistrările DNS particularizate necesare pentru a susține serviciile selectate.

Alternativ, dacă ați modificat înregistrările serverului de nume la Microsoft și aveți un site web, puteți adăuga înregistrări DNS pentru site-ul web în loc să modificați serverele de nume înapoi. Pentru mai multe informații, consultați [Actualizarea înregistrărilor DNS pentru a menține furnizorul curent de găzduire al site-ului web.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


