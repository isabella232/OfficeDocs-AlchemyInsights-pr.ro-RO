---
title: Probleme cu solicitările de token și atributele
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012896"
---
# <a name="issues-with-token-claims-and-attributes"></a>Probleme cu solicitările de token și atributele

**Actualizarea, configurarea sau eliminarea solicitărilor de simboluri**

1. Utilizând un Azure Active Directory (Azure AD), [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) puteți particulariza tipul de solicitare pentru solicitarea de rol în simbolul de răspuns pe care îl primiți după ce autorizați o aplicație.
2. Dezvoltatorii de aplicații pot utiliza solicitări opționale în aplicațiile lor Azure AD pentru a specifica solicitările pe care le doresc în simbolurile trimise aplicației lor. Pentru mai multe informații, consultați [Furnizarea de solicitări opționale pentru aplicația dvs.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configurați solicitările de grup pentru aplicații cu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Dacă utilizați sign-on unic perfect în aplicația dvs., consultați Particularizarea solicitărilor emise în simbolul [SAML pentru aplicațiile de întreprindere.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Maparea atributelor de solicitări**

1. Pentru a configura politica de mapare a solicitărilor folosind PowerShell, consultați Particularizarea solicitărilor omise în simboluri pentru o anumită aplicație [într-o entitate găzduită (Previzualizare).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atributele extensiei schemei directorului furnizează o modalitate de a stoca date suplimentare în Azure Active Directory despre obiectele de utilizator și alte obiecte de director, cum ar fi grupuri, detalii despre entitatea găzduită, entitatea principală de serviciu. Numai atributele de extensie pentru obiectele utilizatorului pot fi utilizate pentru a emite solicitări către aplicații. [Utilizarea atributelor extensiei schemei](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) de director în revendicări descrie cum se utilizează atributele extensiei de schemă de director pentru a trimite date de utilizator aplicațiilor în solicitările de simboluri.

Pentru mai multe informații despre solicitările de simboluri, consultați:

- [Revendicări în tokenurile de acces](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Solicitări într-o id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Solicitări](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) la care vă puteți aștepta în tokenurile DE ID și simbolurile de acces emise de Azure AD B2C
- [Referința la solicitările de token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
