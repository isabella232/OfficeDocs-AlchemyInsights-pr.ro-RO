---
title: 126 Eroarea Obțineți o cutie poștală nu se poate găsi în OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426674"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Eroarea Obțineți o cutie poștală nu a fost găsită în Outlook pe web?

Dacă utilizați Outlook pe web și obțineți o cutie poștală nu **a** fost găsită din eroare, contul pe care l-ați utilizat pentru a vă conecta la Outlook pe web nu are o licență Exchange Online și, prin urmare, nu este asociată nicio cutie poștală cu contul. Administratorul poate atribui o licență contului dvs. urmând acești pași:

1. Deschideți Centrul [de administrare Microsoft 365](https://portal.office.com/adminportal/home#/homepage) și  accesați Utilizatori activi sub secțiunea Utilizatori și selectați utilizatorul care vede eroarea. 

2. Pe pagina de utilizator care  se deschide, accesați secțiunea  Licențe și aplicații, selectați valoarea corespunzătoare Locație și atribuiți o licență care conține Exchange Online (extindeți licența pentru a vedea detaliile). Când terminați, faceți clic pe **Salvare modificări**.

În unele cazuri, dacă licența este atribuită deja unui cont de utilizator, eliminarea și reatriburea licenței ajută la rezolvarea problemei și asigurarea corespunzătoare a accesului la aceasta în sistem: 

- Verificați dacă abonamentele dvs. M365 Exchange Online (și altele, dacă aveți) sunt curente și nu au expirat recent.

După ce v-ați asigurat că abonamentul nu a expirat și i s-a atribuit o licență validă contului de utilizator, poate dura până la 24 de ore pentru ca licența să aibă acces asigurat, deci poate fi necesar să așteptați să se rezolve problema. Pentru mai multe informații, [consultați Atribuirea și gestionarea licențelor.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)