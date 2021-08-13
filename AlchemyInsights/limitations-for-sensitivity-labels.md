---
title: Limitări pentru etichetele de clorți pentru Office în SharePoint și OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813164"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Limitări pentru etichetele de clorți pentru Office în SharePoint și OneDrive

Atunci când activați etichete de sensibilitate pentru Office fișiere din SharePoint și OneDrive, fiți atent la cerințe și limitări, care includ:

- SharePoint și OneDrive nu pot procesa unele fișiere etichetate și criptate din aplicații desktop Office atunci când fișierele conțin date PowerQuery, date stocate de programe de completare particularizate sau părți XML particularizate.
- SharePoint și OneDrive a nu aplica automat etichete de sensibilitate la fișierele existente pe care le-ați criptat deja utilizând etichete Azure Information Protection (AIP). Pentru a aplica etichete de sensibilitate fișierelor criptate: 
    - Asigurați-vă că etichetele AIP au fost migrate și publicate în Centrul Microsoft 365 de conformitate.
    - Descărcați fișierele etichetate, apoi încărcați-le în locația originală SharePoint a OneDrive locația lor.
- Pentru documente criptate, imprimarea nu este acceptată.

Pentru detalii suplimentare despre limitări, consultați [Activarea etichetelor](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)de c Office fișiere în SharePoint și OneDrive .
