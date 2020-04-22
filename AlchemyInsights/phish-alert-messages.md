---
title: 2491 Mesaje de poștă electronică de alertă din politica "Phish livrate din cauza chiriaș sau user suprascrie" politica
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758942"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alertați mesajele de e-mail din politica "Phish livrate din cauza entității găzduite sau a utilizatorului suprascrie"

O politică de alertă implicită denumită "Phish livrate din cauza entității găzduite sau a înlocuirii utilizatorilor" a fost lansată pentru entitățile găzduite cu licențe Office 365 ATP P1 și P2. Dacă ați primit această alertă, iată pașii de investigare:

1. Din mesajul de avertizare, faceți clic pe **Vizualizare avertizare** pentru a accesați pagina **Alerte** din Centrul de securitate & conformitate.

2. Selectați alerta pentru a vedea opțiunea de vizualizare listă **de mesaje** sau Vizualizare mesaje **în Explorer**. Ambele opțiuni vă duc la detaliile mesajului, care include ID-ul mesajului. Rețineți că linkul Explorator amenințări va filtra automat mesajele care corespund criteriilor de alertă. Poate fi necesar să ajustați filtrul de dată în Exploratorul de amenințări.

Mesajul de phishing a fost livrat din cauza unei înlocuiri configurate manual:

- Un expeditor sau un domeniu autorizat setat de utilizator.

- Un expeditor sau un domeniu autorizat setat de administrator într-o politică anti-spam.

- O adresă IP permisă într-o politică de filtrare a conexiunii.

- O regulă de flux de corespondență (cunoscută și ca regulă de transport) care este configurată pentru a permite mesajele.

Dacă credeți că mesajul a fost marcat incorect ca phish, utilizați [programul de completare Mesaj raport](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook pentru a remite mostre de mesaj la Microsoft.
