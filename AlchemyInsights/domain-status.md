---
title: Domain Status (Stare domeniu) - Niciun serviciu selectat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874407"
---
# <a name="domain-status---no-services-selected"></a>Domain Status (Stare domeniu) - Niciun serviciu selectat

**Fără servicii selectate** înseamnă că nu ați selectat niciun serviciu Microsoft 365, cum ar fi Exchange Online, Skype for Business sau Intune și Managementul dispozitivelor mobile pe care Microsoft 365 să le utilizați cu domeniul particularizat. Dacă utilizați o filtrare Exchange hibridă (Exchange local cu Exchange Online) sau filtrarea antispam externă cu Exchange și niciun alt servicii Microsoft, puteți ignora acest mesaj. Starea stării domeniului este disponibilă doar pentru domeniile conectate direct la serviciu.

Pentru a selecta servicii pentru domeniul dvs.:

1. Din **Setări**  >  [**Domenii**](https://admin.microsoft.com/Adminportal/Home), bifați caseta de lângă domeniu cu mesajul de stare **Niciun serviciu selectat**.
1. Selectați **Manage DNS (Gestionare DNS)** pentru a porni Expertul de configurare a domeniului.
    - Dacă alegeți **Adăugați propriile înregistrări DNS**, asigurați-vă că selectați un serviciu atunci când vi se solicită. Mai multe servicii ar putea fi disponibile **sub Opțiuni complexe.**
    - Dacă alegeți **Permiteți ca Microsoft să vă** adauge înregistrările DNS sau Mai multe opțiuni Configurați serviciile online pentru mine, toate serviciile   >   disponibile sunt sugerate și selectate automat.
1. Continuați prin expert pentru a finaliza configurarea DNS și opțiunile de serviciu.
 
Pentru ajutor suplimentar la configurarea domeniului, consultați [Adăugarea de înregistrări DNS pentru a vă conecta domeniul.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

