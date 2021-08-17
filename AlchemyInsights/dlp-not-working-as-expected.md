---
title: DLP nu funcționează așa cum vă așteptați
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079714"
---
# <a name="dlp-not-working-as-expected"></a>DLP nu funcționează așa cum vă așteptați

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

 **Configurarea DLP**

Aveți probleme cu Prevenirea **pierderii datelor (DLP) în** Office 365 nu funcționează așa cum vă așteptați? În acest sens, asigurați-vă că politica **DLP** este configurată corect și că datele conțin ceea ce caută politica **DLP** atunci când este evaluată.
  
Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs. Pentru a configura politicile DLP, utilizați informațiile de [aici.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Ce caută politicile DLP**
  
Atunci când utilizați tipurile **de** informații sensibile predefinite din centrele de securitate și conformitate, politicile DLP caută modele și elemente specifice atunci când detectează aceste tipuri sensibile.
  
- **Tipurile de informații sensibile predefinite**

    Pentru informații despre tipurile sensibile predefinite și despre ce caută o politică DLP atunci când detectează tipul Sensibil, consultați: Ce tipuri de informații sensibile [caută.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Tipuri de informații sensibile la particularizare**

    Dacă încercați să creați tipuri particularizate de informații sensibile, utilizați următorul articol pentru informații despre cum să creați un tip sensibil particularizat: Crearea unui tip de informații [sensibile particularizat.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testarea unei politici DLP**

Pentru a testa datele cu un tip de informații sensibile predefinit sau particularizat, utilizați opțiunea **Tip de test** de sub Tipuri de **informații** sensibile la  >  **clasificări.** Pentru mai multe informații, consultați [Testarea tipurilor de informații sensibile particularizate.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Rapoarte**
  
- Obțineți detalii sensibile despre date [cu rapoartele DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Vedeți detalii specifice ale evenimentului cu un [Raport incident.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
