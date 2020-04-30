---
title: Notificări în Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: ff4c13560b9cbf283e5c6b92a259debdf96cca62
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911914"
---
# <a name="notifications-in-yammer"></a>Notificări în Yammer

Pentru a vă avertiza asupra unei activități noi în conversații relevante, [Yammer trimite notificări](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) prin e-mail sau, dacă utilizați Yammer pe dispozitivul mobil, prin notificări Push. În mod implicit, Yammer vă trimite notificări pentru mai multe tipuri de activitate din rețeaua dvs. Utilizatorii își pot actualiza setările de e-mail prin site-ul web Yammer, iar notificările Push sunt configurate prin aplicația mobilă. 

Yammer a adăugat asistență pentru [e-mailuri interactive din Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Unele mesaje de e-mail (copie mesaj) vor deveni interactive în Outlook pe web. O actualizare viitoare va aduce această caracteristică în alte versiuni de Outlook.

**Tipuri de notificări în Yammer**

- E-mailuri (actualizări de la un grup, cineva vă invită într-un grup, primiți un mesaj în inbox etc.)
- Notificări Push (trimise pe dispozitive mobile când sunteți menționat, primiți un mesaj în inbox etc.)
- Ferestre popup pe desktop (când aveți instalată aplicația desktop Yammer, aceasta va afișa notificările pentru utilizatorii denumiți notificări „toast”.)
- Notificări clopoțel (în interiorul site-ului web Yammer, utilizatorii vor vedea notificări pentru diverse evenimente. Este posibil ca aceste notificări să nu aibă întotdeauna asociată o notificare prin e-mail sau o notificare push.)

Sunt disponibile mai multe [informații detaliate despre notificări](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Gestionarea notificărilor**

Utilizatorii trebuie să își gestioneze propriile notificări. Sunt disponibile informații despre [cum să activați și să dezactivați notificările prin e-mail și mobil Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratorii nu au posibilitatea să dezactiveze toate notificările sau să controleze notificările în numele utilizatorilor. Administratorii pot să [controleze sigla inclusă în mesajele de e-mail și dacă utilizatorii trebuie să confirme mesajele](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) postate prin e-mail.

**Notificări prin e-mail trimise mai multor utilizatori din organizația dvs.**

În unele cazuri, Yammer va trimite o singură notificare prin e-mail, iar aceasta va fi primită de mai mulți utilizatori din organizația dvs. decât se preconiza. Acest lucru se întâmplă când o listă de distribuire sau alt tip de adresă de e-mail care nu este individuală este adăugată la Yammer. Yammer nu știe în toate cazurile, dacă o adresă de e-mail aparține unui singur utilizator sau este o adresă de e-mail care va duce la livrarea unui mesaj de e-mail mai multor destinatari. Atunci când apare această problemă, trebuie să luați măsuri pentru a [suspenda (a dezactiva) utilizatorul nevalid cu acea adresă de e-mail](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) din Yammer. 

Pentru a reduce șansa producerii unei astfel de probleme, ar trebui să:

1. [Impuneți identitatea Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) pentru Yammer.
2. Blocați expeditorii externi să trimită e-mailuri organizației dvs. sau limitați expeditorii la o listă aprobată.

În cazul în care apare această problemă:

1. Identificați destinatarul e-mailului, care ar trebui să corespundă cu utilizatorul din Yammer. De exemplu, all-in-sales@fabrikam.com este un DL pentru toți utilizatorii de vânzări. Acest DL ar putea fi identificat din e-mailul Yammer primit de către utilizatori.
2. Utilizați caracteristica [dezactivare (suspendare) din Administratorul de rețea](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) pentru a suspenda utilizatorul care are adresa de e-mail all-in-sales@fabrikam.com. Suspendarea poate fi anulată, așadar, este mai sigură decât ștergerea. Ștergerea utilizatorului se va produce automat după 90 de zile.
3. Opțional, revizuiți [Export utilizator](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) pentru a identifica adresele de e-mail nespecifice utilizatorilor care ar trebui să fie suspendate.
