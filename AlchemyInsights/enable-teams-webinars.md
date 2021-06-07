---
title: Activarea Teams webinarii
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793781"
---
# <a name="enable-teams-webinars"></a>Activarea Teams webinarii

Webinariile sunt activate implicit. Puteți gestiona cine poate programa și înregistra pentru Teams webinars, utilizând Teams PowerShell.

- Toți utilizatorii care pot crea o întâlnire pot crea, de asemenea, o întâlnire webinar. Dacă doriți să gestionați cine poate programa Teams webinarii, *utilizați AllowMeetingRegistration.* 
- În mod implicit, *WhoCanRegister* este activat și setat la **Oricine.** Dacă doriți să dezactivați înregistrarea întâlnirilor, *setați AllowMeetingRegistration* la **False**.

Pentru a modifica aceste setări, trebuie să [instalați Teams PowerShell.](/microsoftteams/teams-powershell-install) De asemenea, politicile de întâlnire sunt impuse Teams webinarii. De exemplu, dacă asocierea anonimă este dezactivată în setările întâlnirii, utilizatorii anonimi nu se pot alătura la webinarii.

Pentru a afla mai multe despre configurarea cine se poate înregistra pentru webinarii, consultați [Configurarea cine se poate înregistra pentru webinarii.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Pentru mai multe informații despre setările pentru Liste Microsoft, consultați [Controlați setările pentru Liste Microsoft.](/sharepoint/control-lists)