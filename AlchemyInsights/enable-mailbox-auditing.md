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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="f5772-102">Activați auditarea cutiei poștale</span><span class="sxs-lookup"><span data-stu-id="f5772-102">Enable mailbox auditing</span></span>

<span data-ttu-id="f5772-103">Pentru a activa Mailbox audit pentru un singur utilizator sau o organizație întreagă următoarele cmdlet-uri trebuie să fie executat de la distanță Power Shell:</span><span class="sxs-lookup"><span data-stu-id="f5772-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="f5772-104">**Utilizator unic**</span><span class="sxs-lookup"><span data-stu-id="f5772-104">**Single User**</span></span>
  
<span data-ttu-id="f5772-105">Set-Mailbox-identitate "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="f5772-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="f5772-106">**Organizaţie**</span><span class="sxs-lookup"><span data-stu-id="f5772-106">**Organization**</span></span>
  
<span data-ttu-id="f5772-107">Get-cutie poștală-ResultSize nelimitat-filtru {RecipientTypeDetails-EQ "UserMailbox"} | Set-cutie poștală-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="f5772-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="f5772-108">află mai multe</span><span class="sxs-lookup"><span data-stu-id="f5772-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

