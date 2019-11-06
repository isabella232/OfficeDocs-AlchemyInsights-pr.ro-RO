---
title: 2609-reținere-sau-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994088"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Imposibil de șters elemente în SharePoint Online sau OneDrive for Business

Tu sau utilizatorii pot fi imposibil să ștergeți elemente în SharePoint Online sau OneDrive for Business, deoarece o politică de retenție, etichetă de conservare sau eDiscovery Hold se aplică la un SharePoint de OneDrive site-ul sau la un anumit element. Aceasta include imposibilitatea de a șterge un document, o versiune de document, un folder, o bibliotecă de documente, o listă, o aplicație, un site sau o colecție de site-uri. Iată câteva exemple de mesaje de eroare pe care le-ați primit dacă încercați să ștergeți un element care este reținut:

- "Acest site nu poate fi șters, deoarece este inclus într-o politică de așteptare sau retenție eDiscovery"
- "Acest site are o politică de conformitate setată la blocarea ștergerii"
- "O politică de conformitate blochează în prezent această ștergere de site-ul"
- "Această colecție de site-ul nu poate fi șters, deoarece conține site-uri care sunt incluse într-o politică de așteptare sau retenție eDiscovery"
- "Trebuie să ștergeți toate elementele din acest folder înainte de a șterge folderul"
- "Versiunile de acest element nu pot fi șterse, deoarece este în așteptare sau retenție politica"
- "Elementul nu poate fi șters în așteptare"
- "Eticheta care se aplică la acest element împiedică editarea sau ștergerea"
- "Lista nu poate fi ștearsă în timp ce în așteptare sau Politica de retenție"
- "Lista nu poate fi ștearsă dacă este blocată sau dacă se aplică o politică de retenție"

Pentru a șterge elementele dintr-unul dintre aceste scenarii, trebuie eliminată Politica de retenție, eticheta de conservare sau reținerea eDiscovery (sau un site trebuie să fie exclus dintr-o politică de retenție). Trebuie să dezactivați sau să excludeți respectiva așteptare care cauzează această problemă. După ce se elimină o politică de retenție sau o așteptare, poate dura până la 24 de ore pentru ca modificarea să aibă efect. 

Pentru informații despre diferitele caracteristici de retenție și așteptare care pot fi aplicate la site-uri SharePoint și conturi OneDrive, consultați unul dintre următoarele subiecte.

- [Prezentare generală a politicilor de conservare](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Prezentare generală a etichetelor de retenție](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Gestionați deține în Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery deține](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Politicile de închidere și ștergere a site-ului moștenite](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
