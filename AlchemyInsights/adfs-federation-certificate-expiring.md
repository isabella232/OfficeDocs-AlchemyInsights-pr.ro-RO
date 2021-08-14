---
title: Certificat de federalizare ADFS care expiră
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952981"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificat de federalizare ADFS care expiră

Pentru a rezolva această problemă, urmați acești pași:
  
1. Instalați modulul Microsoft Azure Active Directory pentru Windows PowerShell pe computer (dacă modulul nu este deja instalat). Pentru a face acest lucru, [accesați Gestionarea Azure AD utilizând Windows PowerShell](https://aka.ms/aadposh).

2. Urmați pașii din secțiunea "Scenariul 1: Certificatul de semnare a simbolurilor AD FS a expirat" din eroarea "A existat o problemă la accesarea [site-ului" din AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)atunci când un utilizator federativ se conecta la Microsoft 365, Azure sau Intune.

3. Urmați pașii [din Actualizarea sau repararea setărilor unui domeniu federativ în Microsoft, Azure sau Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Pentru a afla mai multe despre reînnoirea certificatelor de federalizare, consultați [Reînnoirea certificatelor](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)de federalizare pentru Microsoft 365 și Azure Active Directory .
