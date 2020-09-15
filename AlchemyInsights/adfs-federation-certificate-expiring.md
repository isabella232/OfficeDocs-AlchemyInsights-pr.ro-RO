---
title: Certificat de federalizare ADFS care expiră
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686761"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificat de federalizare ADFS care expiră

Pentru a rezolva această problemă, urmați acești pași:
  
1. Instalați modulul Microsoft Azure Active Directory pentru Windows PowerShell pe computer (dacă modulul nu este deja instalat). Pentru a face acest lucru, accesați [gestionarea AZURE AD utilizând Windows PowerShell](https://aka.ms/aadposh).

2. Urmați pașii din "scenariul 1: certificatul AD FS-semnarea certificatului a expirat" secțiunea ["a apărut o problemă la accesarea site-ului" din AD FS atunci când un utilizator federativ se conectează la Microsoft 365, Azure sau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Urmați pașii din [actualizarea sau repararea setărilor unui domeniu federativ în Microsoft, Azure sau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Pentru a afla mai multe despre reînnoirea certificatelor de federalizare, consultați [reînnoirea certificatelor de Federation pentru Microsoft 365 și Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
