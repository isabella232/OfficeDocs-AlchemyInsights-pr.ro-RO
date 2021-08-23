---
title: Dezactivarea remiterii clientului TLS1.0 și TLS 1.1 pentru SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455122"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Dezactivarea remiterii clientului TLS1.0 și TLS 1.1 pentru SMTP AUTH

Am început recent dezactivarea TLS1.0 și TLS 1.1 pentru remiterea clientului SMTP AUTH. 

Dacă ați configurat un dispozitiv, o aplicație sau un server care trimite e-mail la Microsoft 365 utilizând metoda de remitere a clientului SMTP AUTH, asigurați-vă că dispozitivul, aplicația sau serverul dvs. acceptă TLS 1.2 pentru SMTP. 