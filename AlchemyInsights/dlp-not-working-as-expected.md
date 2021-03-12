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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707822"
---
# <a name="dlp-not-working-as-expected"></a>DLP nu funcționează așa cum vă așteptați

**Important**: în timpul acestor vremuri fără precedent, vom lua măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân extrem de disponibile. Vizitați [Ajustări temporare de caracteristici SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

 **Configurarea DLP**

Aveți probleme cu **prevenirea pierderii datelor (DLP)** în Office 365 nu funcționează așa cum vă așteptați? Dacă este așa, asigurați-vă că **Politica DLP** este configurată corect și că datele conțin ceea ce caută **Politica DLP** atunci când este evaluată.
  
Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs. Pentru a configura politicile DLP, utilizați informațiile de [aici](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Ce caută politicile DLP**
  
Atunci când utilizați **tipurile de informații sensibile predefinite** din centrele de securitate și conformitate, politicile DLP caută anumite modele și elemente atunci când detectează aceste tipuri sensibile.
  
- **Tipuri de informații sensibile predefinite**

    Pentru informații despre tipurile sensibile predefinite și ce caută o politică DLP atunci când detectează tipul sensibil, consultați: [ce caută tipurile sensibile de informații](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipuri de informații sensibile la comandă**

    Dacă încercați să creați tipuri de informații sensibile particularizate, utilizați următorul articol pentru informații despre cum să creați un tip sensibil particularizat: [Creați un tip de informații sensibile la comandă](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testarea unei politici DLP**

Pentru a testa datele cu un tip de informație predefinit sau particularizat, utilizați opțiunea **tip test** **sub**  >  **Categorii informații sensibile**. Pentru mai multe informații, consultați [testarea tipurilor de informații sensibile particularizate](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapoarte**
  
- Obțineți informații sensibile despre date cu [rapoartele DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Vedeți detaliile specifice ale evenimentului cu un [raport de incident](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
