---
title: Activați auditarea cutiei poștale
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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736265"
---
# <a name="enable-mailbox-auditing"></a>Activați auditarea cutiei poștale

Pentru a activa Mailbox audit pentru un singur utilizator sau o organizație întreagă următoarele cmdlet-uri trebuie să fie executat de la distanță Power Shell:
  
 **Utilizator unic**
  
Set-Mailbox-identitate "Jane Dow"-AuditEnabled $true
  
 **Organizaţie**
  
Get-cutie poștală-ResultSize nelimitat-filtru {RecipientTypeDetails-EQ "UserMailbox"} | Set-cutie poștală-AuditEnabled $true
  
[află mai multe](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

