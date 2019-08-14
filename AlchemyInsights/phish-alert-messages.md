---
title: Mesaje de e-mail de alertă 2491 la politica Phish livrate din cauza locatarul sau utilizatorul suprascrie
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391468"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Mesaje de alertă e-mail la politica Phish livrate din cauza locatarul sau utilizatorul suprascrie

O politică de alertă implicit numit "Phish pronunţată din cauza locatarul sau utilizatorul suprascrie" a fost rulat pentru a chiriaşilor cu Office 365 de ATP P1 şi P2 licenţe. În cazul în care aţi primit această avertizare, aici sunt paşii pentru a investiga:

1. Din mesajul de alertă, faceţi clic pe **Vezi alertă** pentru a merge la pagina **alerte** în securitate & centru de conformitate.

2. Selectaþi Alertaþi pentru a vedea opţiunea de a **lista de mesaje Vezi** sau **vizualizarea mesajelor în Explorer**. Ambele aceste opţiuni vă duce la detaliile mesajului, care include identitate de mesaj. Reţineţi că link-ul de ameninţare Explorer automat va filtra mesajele care se potrivesc criteriilor de alertă. Trebuie să se adapteze filtru dată în ameninţare Explorer.

Mesaj de înşelăciune a fost livrat din cauza o suprascrie configurat manual:

- Un permis expeditorului sau domeniu stabilit de utilizator.

- Un permis expeditorului sau domeniu de admin în o politică anti-spam.

- O adresă IP permise într-o politică de filtru de conexiune.

- Mail fluxul de regulă (de asemenea cunoscut ca o regulă de transport) care este configurat pentru a permite mesajelor în.

Dacă credeţi că mesajul a fost marcat incorect ca phish, utilizaţi Outlook [program de completare raport mesaj](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) să prezinte probe mesaj către Microsoft.
