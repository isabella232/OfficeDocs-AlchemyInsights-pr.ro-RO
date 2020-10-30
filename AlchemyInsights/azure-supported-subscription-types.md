---
title: Tipuri de abonament acceptate
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807977"
---
# <a name="supported-subscription-types"></a>Tipuri de abonament acceptate

Consultați tipurile de abonament acceptate pentru a continua mai departe.

[Tipuri de abonament acceptate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transferați proprietatea de facturare**

Portalul Azure ca [administrator de cont](https://ms.portal.azure.com/) al contului de facturare care are abonamentul pe care doriți să-l transferați

- Căutați în **gestionarea costurilor + facturare** . Selectați **abonamente** din panoul din stânga. În funcție de Access, poate fi necesar să selectați un domeniu de facturare, apoi **abonamente** sau **abonamente Azure** .
- Selectați transferați proprietatea de facturare pentru abonamentul pe care doriți să-l transferați
- Introduceți adresa de e-mail a unui utilizator care este administrator de facturare al contului care va fi noul proprietar pentru abonament, apoi selectați **Trimitere solicitare de transfer**
- Utilizatorul primește un e-mail cu instrucțiuni pentru a revizui solicitarea de transfer. Pentru a aproba solicitarea de transfer, utilizatorul selectează linkul din e-mail și urmează instrucțiunile.

Notă: dacă transferați proprietatea de facturare a abonamentului la un cont de utilizator într-o altă entitate găzduită Azure AD [, toate](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) atribuirile pentru gestionarea resurselor din abonament sunt eliminate definitiv. Doar noul proprietar va avea acces la gestionarea resurselor din abonament. Pentru mai multe informații, consultați [transferul abonamentului la un utilizator într-o altă entitate găzduită AZURE AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Transferarea dreptului de proprietate asupra abonamentului**

Abonamentul de transfer al dreptului de proprietate pentru drepturile de acces (RBAC) pentru a gestiona resursele din abonament își pierde accesul. Pentru mai multe informații despre adăugarea unui abonament existent la o entitate găzduită, consultați [asocierea sau adăugarea unui abonament Azure la Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Transferul abonamentului cu o sumă restantă existentă din ciclul de facturare curent nu va fi transferat la noul instrument de plată din contul nou. Singurele informații disponibile pentru utilizatori în cont nou sunt costurile pentru ultima lună pentru abonamentul dumneavoastră. Restul istoricului de utilizare și facturare nu se transferă cu abonamentul.
- Transferarea dreptului de proprietate asupra abonamentelor pentru contracte de întreprindere (EA) este acceptată în prezent doar în portalul de contracte de întreprindere
- Transferarea unui abonament orientat către credit, cum ar fi Visual Studio, BizSpark, Microsoft Partner Network unui utilizator nou necesită să aibă o licență de rețea de parteneri Visual Studio/Microsoft pentru a accepta solicitarea de transfer
- Toate resursele, cum ar fi mașini virtuale, discuri și site-uri web se transferă cu succes la contul nou. Următoarele resurse pot fi afectate într-un transfer de abonamente pentru entități găzduite:

**Servicii de domeniu Azure AD**

Bolti cheie Azure

- [Utilizatorii și bazele de date SQL asociate](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) pot fi afectate, mai ales dacă clientul utilizează o autentificare Azure Active Directory asociate
- **Serviciile de aplicații** configurate cu autentificarea Azure Active Directory pot fi afectate
- **Echipa Visual Studio** Conturile de servicii conectate la abonamentele Azure pot pierde temporar accesul atunci când este anulat abonamentul Azure conectat

**Documente recomandate**

Pașii după acceptarea proprietății de facturare:

- Pentru a păstra proprietatea de facturare, dar modificați tipul abonamentului, consultați: [Comutați abonamentul Azure la altă ofertă](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transferați Visual Studio, Microsoft Partner Network (MPN) și plătiți pe măsură ce accesați abonamente Dev/test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transferarea dreptului de proprietate al facturilor la abonamentele Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Întrebări frecvente despre proprietatea transfer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Depanarea problemelor legate de proprietatea transfer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)