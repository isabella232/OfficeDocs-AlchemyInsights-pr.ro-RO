---
title: Acces cu abonament
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999252"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nu se poate conecta Azure, din cauza problemelor de browser (browserul se blochează, continuă să se rotească, nu se încarcă etc.)

Este posibil să fiți afectat de o des outage. Verificați dacă există o des out: [Azure Health Status (Stare Azure Health).](https://status.azure.com/status/history/)

Deconectați-vă de la toate sesiunile Azure active. Porniți un mod in-private sau incognito al browserului web.

Puteți, de asemenea, să încercați să Reîmprospătați browserul, să utilizați alt browser, să ștergeți modulele cookie din cache dacă de mai sus nu funcționează.

Aflați mai multe: [Depanarea problemelor de conectare](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nu se pot accesa abonamentele**

În portalul [Azure,](https://portal.azure.com/)asigurați-vă că este selectat directorul Azure corect din contul din dreapta sus.

În Centrul [de conturi Azure,](https://account.windowsazure.com/Subscriptions)asigurați-vă că acesta este administratorul de cont utilizat.

Aflați mai multe: [Depanarea nu a fost găsită pentru abonamente](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nu se poate accesa istoricul de facturare**

Administratorul de cont trebuie să se asigure că utilizatorul care accesează informațiile de facturare este adăugat în directorul Azure Active ca utilizator invitat: Adăugarea sau ștergerea [unui utilizator nou.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Utilizatorului trebuie să i se atribuie un rol de administrator global: [Atribuirea unui rol utilizatorilor.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

După aceasta, utilizatorului i se poate acorda acces de facturare utilizând politici RBAC: [Acordarea accesului la facturare.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documente recomandate**

-   [Nu mă pot conecta pentru a-mi gestiona abonamentul Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)