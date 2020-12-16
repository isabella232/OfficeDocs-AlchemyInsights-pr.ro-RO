---
title: Transfer servicii-mutați toate serviciile RDFE la un alt abonament
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692174"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer servicii-mutați toate serviciile RDFE la un alt abonament

**Mutarea resurselor**

Resursele Azure pot fi mutate la un alt abonament Azure sau la un grup de resurse sub același abonament utilizând Azure portal, Azure PowerShell, Azure CLI sau REST API pentru a muta resursele.

Înainte de a putea muta resursele, consultați:

- [Listă de verificare înainte de mutarea resurselor](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servicii care pot fi mutate](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cum se validează mutarea](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Mutarea ghidării pentru servicii](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Pentru a muta resursele existente într-un alt grup de resurse sau abonament, puteți utiliza:

- [Portalul Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [CLI Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [mutați resursele Azure într-un alt grup de resurse sau abonament](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Depanarea erorilor cu Azure Resource Manager**

Consultați articolele de mai jos pentru a afla despre unele erori comune de implementare Azure și a primi informații pentru a le rezolva. Dacă nu găsiți codul de eroare pentru eroarea de implementare, consultați [Găsirea codului de eroare](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Depanarea erorilor de implementare](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Depanarea mutării resurselor Azure în grup de resurse noi sau abonament](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Rețineți că, dacă doriți să faceți upgrade abonamentului Azure, cum ar fi trecerea de la gratuit la plată-ca-Go, va trebui să efectuați conversia abonamentului.

- Pentru a face upgrade la o versiune de încercare gratuită, consultați [upgrade-ul versiunii de încercare gratuite sau Microsoft imaginați-vă abonamentul Azure la plată-ca-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Pentru a modifica un cont pay-as-Go, consultați [Modificarea abonamentului Azure pay-as-Go la o altă ofertă](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Pentru a adăuga sau a asocia un abonament Azure la entitatea găzduită Azure Active Directory:**

1. Conectați-vă și selectați abonamentul pe care doriți să-l utilizați din [pagina Abonamente din Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Selectați **Modificați directorul**.
3. Revizuiți avertismentele care apar, apoi selectați **modificare**.
4. Directorul este modificat pentru abonament și veți primi un mesaj de succes.
5. Utilizați comutatorul *Director* pentru a merge la noul director. Este posibil să dureze până la 10 minute pentru ca totul să se afișeze corect.

**Documente recomandate**

- [Transferul dreptului de proprietate asupra unui abonament Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mutarea resurselor în grup de resurse sau abonament nou](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gestionarea resurselor utilizând Azure portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
