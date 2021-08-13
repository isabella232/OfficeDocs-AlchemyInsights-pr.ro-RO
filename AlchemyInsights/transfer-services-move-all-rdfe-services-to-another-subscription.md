---
title: Transfer Services - Mutarea tuturor serviciilor RDFE într-un alt abonament
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940079"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services - Mutarea tuturor serviciilor RDFE într-un alt abonament

**Mutarea resurselor**

Resursele Azure pot fi mutate în alt abonament Azure sau grup de resurse în același abonament, utilizând portalul Azure, Azure PowerShell, Azure CLI sau API REST pentru a muta resursele.

Înainte de a putea muta resursele, consultați:

- [Listă de verificare înainte de mutarea resurselor](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servicii care pot fi mutate](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cum se validează mutarea](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Instrucțiuni pentru mutarea serviciilor](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Pentru a muta resursele existente la alt grup de resurse sau abonament, puteți utiliza:

- [Portalul Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [Mutarea resurselor Azure într-un alt grup de resurse sau abonament](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Depanarea erorilor cu Azure Resource Manager**

Consultați articolele de mai jos pentru a afla despre unele erori comune de implementare Azure și a primi informații pentru a le rezolva. Dacă nu găsiți codul de eroare pentru eroarea de implementare, consultați [Găsirea codului de eroare](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Depanarea erorilor de implementare](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Depanarea mutării resurselor Azure în noul grup de resurse sau abonament](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Rețineți că dacă preferați să faceți upgrade abonamentului Azure, de exemplu, să treceți de la gratuit la cu plată, va trebui să efectuați conversia abonamentului.

- Pentru a face upgrade unei încercări gratuite, consultați Upgrade-ul abonamentului Microsoft Imagine Azure gratuit la [Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Pentru a schimba un cont de plată pe loc, consultați Modificarea abonamentului [Azure Pay-As-You-Go la o altă ofertă.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Pentru a adăuga sau a asocia un abonament Azure la entitatea Azure Active Directory găzduită:**

1. Conectați-vă și selectați abonamentul pe care doriți să-l utilizați [din pagina Abonamente din portalul Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Selectați **Schimbați directorul.**
3. Revizuiți orice avertisment care apare, apoi selectați **Modificare**.
4. Directorul este schimbat pentru abonament și veți primi un mesaj de succes.
5. Utilizați *comutatorul* de director pentru a vă duce la noul director. Poate dura până la 10 minute pentru ca totul să se afișează corect.

**Documente recomandate**

- [Transferul proprietății unui abonament Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Mutarea resurselor într-un grup de resurse nou sau într-un nou abonament](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gestionarea resurselor utilizând portalul Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
