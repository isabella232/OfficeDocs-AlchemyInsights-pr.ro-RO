---
title: DLP nu funcționează conform așteptărilor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507490"
---
# <a name="dlp-not-working-as-expected"></a>DLP nu funcționează conform așteptărilor

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

 **Configurarea DLP**

Aveți probleme cu **prevenirea pierderilor de date (DLP)** în Office 365 nu funcționează conform așteptărilor? Dacă da, asigurați-vă că **politica DLP** este configurat corect și că datele conține ceea ce **politica DLP** este în căutarea atunci când este evaluat.
  
Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs. Pentru a parametriza politicile DLP, utilizați informațiile [aici](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Ce caută politicile DLP**
  
Atunci când utilizați **tipurile de informații sensibile încorporate** în centrele de securitate și conformitate, politicile DLP caută anumite modele și elemente atunci când detectează aceste tipuri sensibile.
  
- **Tipuri de informații sensibile încorporate**

    Pentru informații despre tipurile sensibile încorporate și ce caută o politică DLP la detectarea tipului Sensibil, consultați: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipuri de informații sensibile particularizate**

    Dacă încercați să creați tipuri de informații sensibile particularizate, utilizați următorul articol pentru informații despre se creează un tip sensibil particularizat: [Creați un tip de informații sensibile particularizate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testarea unei politici DLP**

Pentru a testa datele cu un tip de informații sensibile predefinite sau particularizate, utilizați opțiunea **Tip test** din **Clasificări**  >  **Tipuri de informații sensibile**. Pentru mai multe informații, consultați [Testarea tipurilor de informații sensibile particularizate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapoarte**
  
- Obțineți informații sensibile despre date cu [rapoarteLE DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- A se vedea detaliile specifice ale evenimentului cu un [raport de incident](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
