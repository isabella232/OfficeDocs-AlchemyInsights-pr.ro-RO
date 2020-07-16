---
title: Problemă la deschiderea sau descărcarea fișierelor în Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148338"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problemă la deschiderea sau descărcarea fișierelor în Yammer

Clasic Yammer acceptă mai multe opțiuni pentru încărcările de fișiere în mesaje și grupuri. În funcție de configurația rețelei, fișierele sunt implicite pentru stocarea în SharePoint.

Selectorul de fișiere din noul Yammer nu acceptă încă toate opțiunile disponibile în Yammer clasic. O actualizare viitoare va adăuga caracteristici suplimentare. Pentru mai multe informații, consultați [Atașarea unui fișier sau a unei imagini la o postare de conversație Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Imposibil de deschis sau descărcat un fișier**  

Este posibil ca un fișier să se încarce în Yammer, dar și să se conecteze la un fișier din SharePoint Online. Pentru a depana, mai întâi trebuie să determinați locația fișierului. Dacă fișierul a fost încărcat în Yammer, acesta va avea un URL *.yammer.com. Asigurați-vă că adresele URL și IP necesare sunt deblocate. Pentru mai multe informații, a se vedea blog post [Folosind greu codificate adrese IP pentru Yammer nu este recomandat](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Verificați dacă un utilizator care este, de asemenea, un administrator global poate descărca fișierul. Dacă fișierul este privat, poate fi necesar să utilizați Modul conținut privat. Pentru mai multe informații, consultați [Monitorizarea conținutului privat în Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Oaspeți și fișiere la nivel de rețea Yammer în SharePoint Online**  

[Oaspeții de la nivel de rețea din Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nu utilizează Azure AD B2B și sunt interni pentru serviciul Yammer, astfel încât nu pot accesa fișierele Yammer stocate în SharePoint. Creați un utilizator AAD B2B extern care poate accesa biblioteci de documente în SharePoint Online utilizând acea identitate. Pentru informații despre viitoarea asistență pentru oaspeții Azure AD B2B în Yammer, consultați [Asistență pentru clienți de la afaceri la afaceri (B2B) în Yammer Preview - Termeni și întrebări frecvente pentru clienți.](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)