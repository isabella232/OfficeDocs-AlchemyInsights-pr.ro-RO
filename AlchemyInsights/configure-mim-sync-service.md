---
title: Configurarea serviciului de sincronizare MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482900"
---
# <a name="configure-mim-sync-service"></a>Configurarea serviciului de sincronizare MIM

Serviciul de sincronizare Microsoft Identity Manager (MIM) este o componentă a MIM. Este un serviciu local centralizat care stochează și integrează informații pentru organizațiile care au mai multe directoare și baze de date locale. Este posibil să reușiți să rezolvați problema cu sincronizarea MIM dacă problema a fost adresată într-o actualizare recentă la MIM sau este una dintre celelalte probleme menționate în secțiunea de mai jos.

**Pașii recomandați**

1. Asigurați-vă că utilizați o actualizare recentă a sincronizării MIM și verificați [notele de lansare pentru sincronizarea mim](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) pentru a determina dacă problema a fost rezolvată într-o actualizare.
2. Dacă problema este cu genericul LDAP, generic SQL, Lotus Domino sau Web Services Connector, asigurați-vă că utilizați o actualizare recentă a [conectorilor generici](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Dacă o rulare de sincronizare MIM se oprește cu o eroare, consultați tabelul de [coduri de eroare rulare](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) pentru a determina cauzele potențiale.
4. Dacă rulează se oprește cu **extensia-dll-excepție**, apoi faceți clic pe acele cuvinte pentru a deschide fereastra **Proprietăți obiect spațiu conector** și faceți clic pe **Trasare stivă...** pentru a vedea mai multe informații despre cauza principală, așa cum este descris în [extensia-dll-excepție](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Dacă componenta de notificare de modificare a parolei (PCNS) raportează **eroarea 6025** din jurnalul de evenimente în timpul sincronizării parolei, consultați Ghidul pentru depanarea [erorilor de raportare PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Dacă sincronizarea completă cu agentul de gestionare a serviciului FIM este lentă, bifați setarea **creștere automată** pentru tempdb, așa cum este descris în [Depanarea lentă sau suspendarea sincronizării complete](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Dacă întâmpinați o eroare de server oprit cu crearea nereușită-prin-web-servicii utilizând agentul de gestionare a serviciilor FIM, consultați [asistență-informații: failed-Creation-prin-Web-Services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) pentru o prezentare generală a cauzelor.

