---
title: Configurație virtuală cu servicii de domeniu AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885647"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Configurație virtuală cu servicii de domeniu AAD

Configurarea virtuală cu servicii de domeniu AAD implică următorii pași: 

1. Verificarea stării domeniului în portalul Azure https://aka.ms/aadds-health
2. Verificarea NSG pentru reguli care blochează porturile necesare pentru a se sincroniza în Azure AD Domain Services pe portal https://aka.ms/aadds-networking
3. Pentru a vă asigura că rețeaua virtuală este implementată în aceeași regiune Azure ca domeniu gestionat de domeniul Azure AD Services.
4. Pentru a vă asigura că nu aveți un domeniu existent cu același nume de domeniu disponibil în rețeaua virtuală.

Pentru mai multe detalii despre proiectarea aspectului în rețeaua virtuală Azure pentru a accepta servicii de domeniu AAD, consultați [analiza rețelelor virtuale](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

