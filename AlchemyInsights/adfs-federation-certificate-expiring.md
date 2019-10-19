---
title: Certificat de federalizare ADFS expirând
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737201"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificat de federalizare ADFS expirând

Pentru a rezolva această problemă, urmați acești pași:
  
1. Instalați Microsoft Azure Active Directory Module pentru Windows PowerShell pe computer (dacă modulul nu este deja instalat). Pentru aceasta, du-te pentru a [gestiona AZURE AD utilizând Windows PowerShell](https://aka.ms/aadposh).

2. Urmați pașii din "scenariul 1: AD FS token-semnarea certificatului expirat" secțiunea ["nu a fost o problemă accesarea site-ului" eroare la AD FS atunci când un utilizator federalizate semne în Office 365, Azure sau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Urmați pașii din [actualizarea sau repararea setărilor unui domeniu federalizate în Office 365, Azure sau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Pentru a afla mai multe despre reînnoirea certificatelor de federalizare, consultați [reînnoirea certificatelor de federalizare pentru Office 365 și Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
