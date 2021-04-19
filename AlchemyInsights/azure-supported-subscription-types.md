---
title: Tipurile de abonamente acceptate
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
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820694"
---
# <a name="supported-subscription-types"></a>Tipurile de abonamente acceptate

Revizuiți tipurile de abonamente acceptate pentru a continua.

[Tipurile de abonamente acceptate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transferați proprietatea asupra facturării**

Portalul Azure ca administrator [de cont al contului](https://ms.portal.azure.com/) de facturare care are abonamentul pe care doriți să îl transferați

- Căutați **Management de costuri + Facturare**. Selectați **Abonamente** din panoul din stânga. În funcție de acces, poate fi necesar să selectați un domeniu de facturare, apoi să **Abonamente** sau **Abonamente Azure**.
- Selectați Transferați proprietatea asupra facturării pentru abonamentul pe care doriți să îl transferați
- Introduceți adresa de e-mail a unui utilizator care este administrator de facturare al contului care va fi noul proprietar pentru abonament, apoi selectați trimiteți **solicitarea de transfer**
- Utilizatorul primește un mesaj de e-mail cu instrucțiuni pentru revizuirea solicitării dvs. de transfer. Pentru a aproba solicitarea de transfer, utilizatorul selectează linkul din e-mailul și urmează instrucțiunile.

Notă: Dacă transferați proprietatea de facturare a abonamentului la un cont de utilizator din altă entitate găzduită Azure AD, toate atribuirile de control al accesului bazate pe roluri [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) pentru gestionarea resurselor din abonament sunt eliminate definitiv. Doar noul proprietar va avea acces la gestionarea resurselor din abonament. Pentru mai multe informații, consultați [Transferul abonamentului la un utilizator din altă entitate găzduită Azure AD.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Transferarea proprietății abonamentului**

Cerințe preliminare pentru transferul proprietății pe bază de abonament Acces bazat pe rol (RBAC) pentru a gestiona resursele din abonament își pierd accesul. Pentru mai multe informații despre adăugarea unui abonament existent la o entitate găzduită, consultați Asocierea sau [adăugarea unui abonament Azure la Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

- Transferul abonamentului cu o sumă rest primită existentă din ciclul de facturare curent nu va fi transferat la noul instrument de plată din noul cont. Singurele informații disponibile utilizatorilor din noul cont sunt costul ultimei luni pentru abonamentul dvs. Restul istoricului de utilizare și facturare nu se transferă cu abonamentul.
- Transferul proprietății de facturare a abonamentelor prin Contract Enterprise (EA) este acceptat în prezent doar în Portalul pentru acordul Enterprise
- Transferul unui abonament orientat către credit, cum ar fi Visual Studio, BizSpark, Microsoft Partner Network către un utilizator nou, necesită să aibă o licență de rețea partener Visual Studio/Microsoft pentru a accepta solicitarea de transfer
- Toate resursele, cum ar fi mașinile virtuale, discurile și site-urile web se transferă cu succes în noul cont. Următoarele resurse pot fi afectate într-un transfer de abonamente la mai multe entități găzduite:

**Servicii de domeniu Azure AD**

Seifurile de taste Azure

- [Utilizatorii și bazele de](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) date asociate cu SQL pot fi afectate, mai ales dacă clientul utilizează autentificarea legată de Azure Active Directory
- **Serviciile de aplicație** configurate cu autentificarea Azure Active Directory pot fi afectate
- **Echipa Visual Studio** Conturile de servicii conectate la abonamentele Azure pot pierde temporar accesul atunci când abonamentul Azure conectat este anulat

**Documente recomandate**

Pașii după ce acceptați proprietatea asupra facturării:

- Pentru a păstra proprietatea asupra facturării, dar a modifica tipul abonamentului, consultați: [Comutați abonamentul Azure la o altă ofertă](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transferarea Visual Studio, Microsoft Partner Network (MPN) și plata pe Măsura deplasării a abonamentelor Dev/Test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transferul proprietății asupra facturării pentru abonamentele Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Întrebări frecvente despre transferul de proprietate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Depanarea problemelor de proprietate a transferului](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)