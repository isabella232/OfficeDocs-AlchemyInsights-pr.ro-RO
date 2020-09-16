---
title: 2491 alertați mesajele de e-mail de la politica "phishing livrate din cauza entității găzduite sau a utilizatorului"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728623"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Avertizarea mesajelor de e-mail de la politica "phishing livrate din cauza entității găzduite sau a utilizatorului

O politică de avertizare implicită denumită "phishing livrat din cauza entității găzduite sau a unui utilizator de înlocuire" a fost lansată pentru entități găzduite cu licențe Office 365 ATP P1 și P2. Dacă ați primit această avertizare, Iată pașii de investigat:

1. Din mesajul de avertizare, faceți clic pe **vizualizare avertizare** pentru a merge la pagina **avertizări** din centrul de conformitate & de securitate.

2. Selectați avertizarea pentru a vedea opțiunea de a **vizualiza lista** de mesaje sau a **vizualiza mesajele în Explorer**. Ambele opțiuni vă duc la detaliile mesajului, care include ID-ul mesajului. Rețineți că linkul Threat Explorer va filtra automat mesajele care se potrivește cu criteriile de avertizare. Poate fi necesar să ajustați filtrul de date în Explorer.

Mesajul de phishing a fost livrat din cauza unei supracomenzi configurate manual:

- Un expeditor sau un domeniu permis setat de utilizator.

- Un expeditor sau un domeniu permis setat de administrator într-o politică anti-spam.

- O adresă IP permisă într-o politică de filtrare a conexiunii.

- O regulă de flux de corespondență (denumită și regulă de transport) care este configurată pentru a permite mesajele din.

Dacă considerați că mesajul a fost marcat incorect ca phishing, utilizați programul de [completare pentru mesaje de raport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook pentru a trimite eșantioane de mesaje la Microsoft.
