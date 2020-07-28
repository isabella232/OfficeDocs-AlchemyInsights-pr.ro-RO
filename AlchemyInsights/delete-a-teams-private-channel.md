---
title: Ștergerea unui canal privat Echipe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439917"
---
# <a name="delete-a-teams-private-channel"></a>Ștergerea unui canal privat Echipe

Microsoft este conștient de o problemă la ștergerea unui canal privat Teams dacă aveți politicile de retenție SharePoint activate pentru site-ul SharePoint subiacent. Microsoft lucrează la o remediere. Între timp, puteți utiliza următoarele soluții pentru a șterge canalul privat.

**Excludeți colecția de echipă/site din politica de retenție Sharepoint.**

1. Accesați portalul de administrare Office 365 și selectați **Afișare totală** în panoul de navigare din stânga.
2. Sub **Centre de administrare**, accesați Politica de prevenire a **Security & Compliance**  >  **pierderilor de date**de &  >  **conformitate**.
3. Identificați orice politică care se aplică site-urilor Sharepoint și modificați politica astfel încât site-ul Sharepoint pentru echipa care conține canalul privat SĂ NU fie inclus în politica de retenție.
4. Salvează politica.
    Poate dura până la 24 de ore pentru ca setările de politică să intre în vigoare.
    După ce site-ul a fost exclus, puteți șterge canalul privat.  
    
Este ***posibil*** să puteți șterge canalul privat utilizând Microsoft Teams pe dispozitivul Android. 

Pentru informații SharePoint corelate, consultați [Imposibil de șters elemente din SharePoint Online sau OneDrive pentru business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).