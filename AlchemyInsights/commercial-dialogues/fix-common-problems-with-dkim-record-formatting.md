---
title: Remedierea problemelor obișnuite cu formatarea înregistrării DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750759"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Remedierea problemelor obișnuite cu formatarea înregistrării DKIM

Majoritatea problemelor de configurare DKIM sunt asociate înregistrărilor DNS incorecte.

Pentru a remedia problemele de configurare DKIM, Verificați dacă înregistrarea CNAME DKIM (**nu** este o înregistrare txt) este formatat corect. Pentru mai multe informații, consultați [ce trebuie să faceți pentru a configura manual DKIM în Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Dacă aveți nevoie de ajutor cu înregistrările DNS în general, consultați [crearea de înregistrări DNS la orice furnizor de găzduire DNS pentru Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> După ce creați sau actualizați înregistrările DNS DKIM la serviciul de găzduire DNS pentru domeniul dvs., va trebui să așteptați să se propage înregistrările DNS.
