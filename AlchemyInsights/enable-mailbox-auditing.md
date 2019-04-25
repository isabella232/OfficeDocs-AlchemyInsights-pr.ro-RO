---
title: Activează cutia poştală de audit
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403759"
---
# <a name="enable-mailbox-auditing"></a>Activează cutia poştală de audit

Pentru a activa căsuţa poştală de audit pentru un singur utilizator sau o organizatie intreaga următoarele cmdlet-uri trebuie să fi rulat de Remote Power Shell:
  
 **Monopost**
  
Set-Mailbox - Identity "Jane Dow" - AuditEnabled $true
  
 **Organizarea**
  
Ia-Mailbox - ResultSize nelimitat - filtru {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true
  
[află mai multe](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

