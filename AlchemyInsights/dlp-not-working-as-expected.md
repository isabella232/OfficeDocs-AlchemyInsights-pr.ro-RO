---
title: DLP nu funcționează conform așteptărilor
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977450"
---
# <a name="dlp-not-working-as-expected"></a>DLP nu funcționează conform așteptărilor

**Important:** În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile - vizitați [Ajustări le caracteristică temporară SharePoint Online](https://aka.ms/ODSPAdjustments) pentru mai multe informații.

 **Configurarea DLP**

Aveți probleme cu **prevenirea pierderilor de date (DLP)** în Office 365 nu funcționează conform așteptărilor? Dacă da, asigurați-vă că **politica DLP** este configurat corect și că datele conține ceea ce **politica DLP** este în căutarea atunci când este evaluat.
  
Politicile DLP vă permit să identificați și să protejați informațiile sensibile din organizația dvs. Pentru a parametriza politicile DLP, utilizați informațiile [aici](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Ce caută politicile DLP**
  
Atunci când utilizați **tipurile de informații sensibile predefinite** în Centrul de securitate și conformitate Office 365, politicile DLP caută anumite modele și elemente atunci când detectează aceste tipuri sensibile.
  
- **Tipuri de informații sensibile încorporate**

    Pentru informații despre tipurile sensibile încorporate și ce caută o politică DLP la detectarea tipului Sensibil, consultați: [Ce caută tipurile de informații sensibile](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Tipuri de informații sensibile particularizate**

    Dacă încercați să creați tipuri de informații sensibile particularizate, utilizați următorul articol pentru informații despre se creează un tip sensibil particularizat: [Creați un tip de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testarea unei politici DLP**

Pentru a testa datele cu un tip de informații sensibile predefinite sau particularizate, utilizați opțiunea **Tip test** din **Clasificări** > **Tipuri de informații sensibile**. Pentru mai multe informații, consultați [Testarea tipurilor de informații sensibile particularizate](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapoarte**
  
- Obțineți informații sensibile despre date cu [rapoarteLE DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- A se vedea detaliile specifice ale evenimentului cu un [raport de incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
