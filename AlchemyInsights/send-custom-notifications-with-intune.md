---
title: Trimiteți notificări personalizate cu Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992324"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>să trimiteți notificări personalizate utilizatorilor de dispozitive iOS și Android gestionate

Notificările particularizate pentru Intune sunt procesate de aplicația portal de companie pe dispozitivul unui utilizator. Aplicația apoi creează notificarea Push pe acel dispozitiv.

Următoarele sunt premise pentru dispozitiv pentru a accepta primirea notificărilor particularizate și pentru ca aplicația să creeze apoi notificarea Push:

- Dispozitivul trebuie să aibă instalată aplicația portal de companie.  

- Dispozitivul trebuie să permită aplicației portal companie să trimită notificări Push. Când aplicația este instalată sau actualizată, va solicita utilizatorului să permită notificări.

- Dispozitivele Android trebuie să aibă instalat serviciile Google Play.

- Dispozitivul trebuie să fie înscris cu Intune.

Pentru mai multe informații, inclusiv să trimiteți un mesaj, consultați [documentația caracteristică](https://docs.microsoft.com/intune/custom-notifications).
