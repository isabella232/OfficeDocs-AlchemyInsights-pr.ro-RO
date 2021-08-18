---
title: 2491 Mesajele de e-mail de avertizare de la politica "Mesaje de e-mail livrate ca urmare a entității găzduite sau a înlocuirii utilizatorului"
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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316370"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Alert email messages from the "Phish Delivered due to tenant or user override" policy

O politică de avertizare implicită denumită Mesaj livrat datorită entității **găzduite** sau înlocuirii utilizatorilor este disponibilă în organizațiile cu Microsoft Defender pentru Office 365 P1 și P2. Dacă ați primit această avertizare, iată pașii pentru a investiga:

1. Din mesajul de avertizare, faceți **clic pe** Vizualizare avertizare pentru **a vă** duce la pagina Avertizări Microsoft 365 Defender portal.

2. Selectați avertizarea pentru a vedea opțiunea vizualizarea **listei de mesaje** sau **Vizualizarea mesajelor în Explorer.** Ambele opțiuni vă duc la detaliile mesajului, care include ID-ul de mesaj. Rețineți că linkul Threat Explorer va filtra automat mesajele care se potrivesc cu criteriile de avertizare. Poate fi necesar să ajustați filtrul de dată în Threat Explorer.

Mesajul de înșelăciune a fost livrat din cauza unei înlocuiri configurate manual:

- Un expeditor sau un domeniu permis setat de utilizator.
- Un expeditor sau un domeniu permis setate de administrator într-o politică antispam.
- O adresă IP permisă într-o politică de filtrare a conexiunii.
- O regulă de flux de corespondență (numită și regulă de transport) care este configurată pentru a permite mesajele.

Dacă credeți că mesajul a fost marcat incorect ca phishing, utilizați [Remiterea administratorului](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) pentru a raporta mesajul la Microsoft.

Utilizatorii pot utiliza [programul de completare Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) sau programul de completare Report Phishing Outlook pentru a remite exemple de mesaje la Microsoft.
