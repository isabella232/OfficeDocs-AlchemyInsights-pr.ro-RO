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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932634"
---
# <a name="dlp-not-working-as-expected"></a>DLP nu funcționează conform așteptărilor

**Important:** Mulți clienți SharePoint Online și OneDrive executați aplicații critice pentru afaceri împotriva serviciului care se execută în fundal. Acestea includ migrarea conținutului, Prevenirea pierderilor de date (DLP) și soluțiide copiere de rezervă. În timpul acestor momente fără precedent, luăm măsuri pentru a ne asigura că serviciile SharePoint Online și OneDrive rămân foarte disponibile și fiabile pentru utilizatorii care depind de serviciu mai mult ca niciodată în scenarii de lucru la distanță.

În sprijinul acestui obiectiv, am implementat limite mai stricte de limitare a aplicațiilor de fundal (migrare, DLP și soluții de backup) în timpul orelor de zi din timpul săptămânii. Ar trebui să vă așteptați ca aceste aplicații să obțină un debit foarte limitat în aceste perioade. Cu toate acestea, în timpul orelor de seară și de weekend pentru regiune, serviciul va fi gata să proceseze un volum semnificativ mai mare de solicitări din aplicațiile de fundal.

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
