---
title: Transferarea proprietății Azure Billing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036108"
---
# <a name="transfer-azure-billing-ownership"></a>Transferarea proprietății Azure Billing

Conectați-vă la [Portalul Azure](https://portal.azure.com/) ca administrator al contului de facturare care are abonamentul pe care doriți să-l transferați. Dacă nu sunteți sigur dacă sunteți administrator sau dacă trebuie să determinați cine este, consultați [Determinați administrator de facturare a contului](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Căutare _Gestionare costuri + Facturare_.
1. Selectați **Abonamente** din panoul din stânga. În funcție de acces, poate fi necesar să selectați un domeniu de facturare, apoi să **Abonamente** sau **Abonamente Azure**.
1. Selectați **Transferul de proprietate de facturare** pentru abonamentul pe care doriți să-l transferați.
1. Introduceți adresa de e-mail a unui utilizator care este administrator de facturare al contului care va fi proprietarul nou pentru abonament, apoi selectați **Trimitere solicitare de transfer**.
1. Utilizatorul primește un mesaj de e-mail cu instrucțiuni pentru revizuirea solicitării dvs. de transfer. Pentru a aproba solicitarea de transfer, utilizatorul selectează linkul din e-mailul și urmează instrucțiunile.

Vă rugăm să rețineți că, dacă transferați proprietatea de facturare a abonamentului dvs. într-un cont de utilizator dintr-o altă entitate găzduită Azure AD, toate atribuirile de gestionare a resurselor de [control al accesului bazat pe roluri (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) sunt eliminate definitiv. Doar noul proprietar va avea acces la gestionarea resurselor din abonament. Pentru mai multe informații despre cum se modifică directorul pentru un abonament, consultați [Transferul abonamentului la un utilizator din altă entitate găzduită Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Un impact important asupra facturilor dvs.**_: dacă ați transferat proprietatea de facturare pentru un abonament Azure, costurile vor fi evaluate în mod pro. Veți putea să accesați facturile după cum urmează:  

1. Selectați abonamentul din [pagina Abonamente](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) în portalul Azure, ca [utilizator cu acces la facturi](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), apoi selectați **Facturi**.
1. Faceți clic pe **Descărcare factură** pentru a vizualiza o copie a facturii PDF. Dacă spune _Nu este disponibil_, consultați [De ce nu văd o factură pentru ultima perioadă de facturare?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. De asemenea, puteți vizualiza utilizarea zilnică, făcând clic pe **perioadă de facturare** pentru a obține un PDF al facturii și o copie a fișierului de utilizare cotidiană (. CSV). Pentru mai multe informații, consultați [Obținerea datelor despre factură și utilizare](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documente recomandate**

- [Transferul de proprietate de facturare pentru un abonament Azure la un alt cont](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Despre transferul proprietății de facturare pentru un abonament Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transferarea Visual Studio, Microsoft Partner Network (MPN) și plata pe Măsura deplasării a abonamentelor Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Întrebări frecvente despre transferul de proprietate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Depanarea problemelor de proprietate a transferului](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
