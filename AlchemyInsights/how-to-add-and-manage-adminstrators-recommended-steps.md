---
title: Cum se adaugă și se gestionează administratorii - pași recomandați
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339044"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Cum se adaugă și se gestionează administratorii - pași recomandați

Pe baza descrierii problemei, am găsit o soluție pentru dvs. Majoritatea clienților au reușit să-și rezolve singuri problema după ce au urmărit documentația.

**Editarea Administratorului de abonament sau a Co-administratorului**

- Administratorul de cont poate edita ambele roluri, în timp ce administratorul de abonament poate schimba doar co-administratorii din [portalul Azure.](https://ms.portal.azure.com/#home)
- [Adăugarea sau modificarea administratorilor de abonament Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Actualizarea Administratorului de abonament sau a Co-Administrator pentru abonamentele interne (AIRS)**

Administratorul de serviciu sau Co-administratorul poate servi singur această acțiune, utilizând următorii pași:

1. Conectați-vă la [portalul Azure și](https://ms.portal.azure.com/#home) faceți clic pe Gestionare costuri **+** Facturare în sistemul blade din stânga.
2. Faceți clic pe articolul de linie cu abonamentul dvs. Astfel se va deschide Prezentarea generală a abonamentului.
3. Pe **blade** abonament, faceți clic pe **Proprietăți**. 
4. Faceți clic **pe butonul Administrator de** servicii.
5. Introduceți e-mailul utilizatorului pe care doriți să-l setați ca Administrator de servicii și faceți clic **pe OK.**

**Adăugare/modificare/eliminare co-administrator**

1. Conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) ca administrator de servicii.
2. Deschideți [Abonamente](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) și selectați un abonament. (Co-administratorii pot fi atribuiți numai în domeniul de abonament.)
3. Navigați la administratorii controlului **Access (IAM)** Clasic: Adăugați un co-administrator pentru a deschide panoul Adăugare  >    >    >   **co-administrator** (dacă opțiunea Adăugare co-administrator este dezactivată, înseamnă că nu aveți permisiuni).
4. Selectați utilizatorul pe care doriți să-l adăugați și faceți clic **pe Adăugare.**

**află mai multe:**
- [Adăugarea unui co-administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Eliminarea unui co-administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Modificarea administratorului de servicii](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Vizualizarea administratorului de cont](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gestionarea accesului utilizând portalul RBAC și Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Adăugarea/ștergerea utilizatorilor utilizând Azure Active Directory (AD)**

Puteți să adăugați utilizatori noi sau să ștergeți utilizatorii existenți din organizația Azure Active Directory (Azure AD):

1. Pentru a adăuga un utilizator nou, conectați-vă [la portalul Azure](https://ms.portal.azure.com/#home) ca administrator de utilizator al organizației.
2. Selectați **Azure Active Directory** selectați **Utilizatori,** apoi faceți clic **pe Utilizator nou.**
3. Pe pagina **Utilizator,** completați informațiile necesare. Faceți **clic pe Creare.** Utilizatorul este creat și adăugat la entitatea dvs. găzduită Azure AD.

**Aflați mai multe:**

- [Adăugarea unui utilizator nou](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Ștergerea unui utilizator](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Adăugarea sau actualizarea informațiilor de profil ale unui utilizator utilizând Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documente recomandate**

- [Ce este controlul accesului bazat pe roluri (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Înțelegeți rolurile diferite din Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Permisiunile rolului de administrator în Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Tutorial: Acordarea accesului pentru un utilizator utilizând RBAC și portalul Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Depanarea RBAC în Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizați-vă resursele cu grupurile de gestionare Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Cum să solicitați o copie a facturii Azure prin e-mail](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Cum se adaugă, actualizează sau elimină un card de credit sau de debit din Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Gestionați (reactivați/anulați/comutați) abonamentul](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



