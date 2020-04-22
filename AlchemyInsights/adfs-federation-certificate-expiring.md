---
title: Certificatul de federalizare ADFS expiră
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710419"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificatul de federalizare ADFS expiră

Pentru a rezolva această problemă, urmați acești pași:
  
1. Instalați Microsoft Azure Active Directory Module pentru Windows PowerShell pe computer (dacă modulul nu este deja instalat). Pentru aceasta, accesați [Gestionarea Azure AD utilizând Windows PowerShell](https://aka.ms/aadposh).

2. Urmați pașii din secțiunea "Scenariul 1: Certificatul de semnare a simbolului AD FS a expirat" din ["A existat o problemă la accesarea site-ului" eroare din AD FS atunci când un utilizator federativ se conectează la Microsoft 365, Azure sau Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Urmați pașii din [Actualizarea sau repararea setărilor unui domeniu federativ în Microsoft, Azure sau Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Pentru a afla mai multe despre reînnoirea certificatelor de federalizare, consultați [Reînnoirea certificatelor de federalizare pentru Microsoft 365 și Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
