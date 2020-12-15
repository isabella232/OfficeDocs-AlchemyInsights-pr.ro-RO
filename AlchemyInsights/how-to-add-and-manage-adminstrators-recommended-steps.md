---
title: Cum să adăugați și să gestionați pașii recomandați adminstrators
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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678874"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Cum să adăugați și să gestionați pașii recomandați adminstrators

**Editarea administratorului de abonament sau a co-administratorului**

- Administratorul de cont poate edita ambele roluri, în timp ce administratorul abonamentului poate modifica doar co-administratorii din [portalul Azure](https://ms.portal.azure.com/#home).
- [Adăugarea sau modificarea administratorilor de abonament Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Actualizați administratorul abonamentului sau Co-Administrator pentru abonamentele interne (DIFUZe)**

Administratorul serviciului sau coadministratorul poate să servească automat această acțiune, utilizând următorii pași:

1. Conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) și faceți clic pe **gestionare costuri + facturare** în lama din stânga.
2. Faceți clic pe elementul linie cu abonamentul dvs. Aceasta deschide prezentarea generală a abonamentului dumneavoastră.
3. Pe lama **abonamentului** , faceți clic pe **Proprietăți**. 
4. Faceți clic pe butonul **administrator serviciu** .
5. Introduceți adresa de e-mail a utilizatorului pe care doriți să-l setați ca administrator de serviciu și faceți clic pe **OK**.

**Adăugare/Modificare/Eliminare co-administrator**

1. Conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) ca administrator de serviciu.
2. Deschideți [abonamente](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) și selectați un abonament. (Co-adminstrators poate fi atribuită doar în domeniul abonamentului.)
3. Navigarea la administratorii Classic **Access Control (iam)**  >    >  **Adăugare**  >  **Adăugare co-administrator** pentru a deschide panoul **Adăugare co-** administrator (dacă opțiunea Adăugare co-administrator este dezactivată, aceasta denotă faptul că nu aveți permisiuni).
4. Selectați utilizatorul pe care doriți să-l adăugați și faceți clic pe **Adăugare**.

**află mai multe:**
- [Adăugarea unui co-administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Eliminarea unui co-administrator](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Modificarea administratorului serviciului](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Vizualizați Administratorul contului](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Gestionarea accesului utilizând RBAC și portalul Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Adăugarea/ștergerea utilizatorilor utilizând Azure Active Directory (AD)**

Puteți să adăugați utilizatori noi sau să ștergeți utilizatori existenți din organizația Azure Active Directory (Azure AD):

1. Pentru a adăuga un utilizator nou, conectați-vă la [portalul Azure](https://ms.portal.azure.com/#home) ca administrator de utilizator al organizației.
2. Selectați **Azure Active Directory**, selectați **utilizatori** , apoi faceți clic pe **utilizator nou**.
3. În pagina **utilizator** , completați informațiile necesare. Faceți clic pe **Creare**. Utilizatorul este creat și adăugat la entitatea găzduită Azure AD.

**Aflați mai multe**:

- [Adăugarea unui utilizator nou](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Ștergerea unui utilizator](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Adăugarea sau actualizarea informațiilor de profil ale unui utilizator utilizând Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Documente recomandate**

- [Ce este controlul Access bazat pe roluri (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Înțelegerea diferitelor roluri din Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Permisiuni pentru rolul de administrator în Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Tutorial: acordarea accesului pentru un utilizator utilizând RBAC și portalul Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Depanarea RBAC în Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organizarea resurselor cu grupurile de gestionare Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Cum să solicitați o copie a facturii Azure prin e-mail](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Cum să adăugați, să actualizați sau să eliminați un card de credit sau de debit din Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Abonament de gestionare (reactivare/anulare/comutare)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



