---
title: Probleme cu revendicările și atributele token
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035970"
---
# <a name="issues-with-token-claims-and-attributes"></a>Probleme cu revendicările și atributele token

**Actualizarea, configurarea sau eliminarea revendicărilor token**

1. Utilizând Azure Active Directory (Azure AD), puteți [particulariza tipul de revendicare pentru revendicarea rolului](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) în simbolul de răspuns pe care îl primiți după ce autorizați o aplicație.
2. Dezvoltatorii de aplicații pot utiliza revendicări opționale în aplicațiile lor Azure AD pentru a specifica ce revendicări doresc în tokenuri trimise aplicației. Pentru mai multe informații, consultați [furnizarea de solicitări opționale la aplicație](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Configurați revendicările de grup pentru aplicațiile cu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Dacă utilizați sign-on unic fără sudură în aplicația dvs., consultați [Particularizarea creanțelor emise în fișierul SAML pentru aplicațiile Enterprise](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Maparea atributului revendicări**

1. Pentru a configura politica de mapare a revendicărilor utilizând PowerShell, consultați [Particularizarea creanțelor emise în tokenuri pentru o anumită aplicație într-o entitate găzduită (Previzualizare)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atributele de extensie a schemelor directoare oferă o modalitate de a stoca date suplimentare în Azure Active Directory pentru obiectele de utilizator și alte obiecte din Director, cum ar fi grupuri, detalii despre entități găzduite, directori de servicii. Numai atributele de extensie pentru obiectele de utilizator pot fi utilizate pentru emiterea de revendicări la aplicații. [Utilizarea atributelor de extensie a schemelor directoare din revendicări](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) descrie modul în care se utilizează atributele de extensie a schemelor directoare pentru trimiterea datelor de utilizator la aplicațiile din revendicările token.

Pentru mai multe informații despre revendicările Token, consultați:

- [Revendicări în jetoanele Access](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Creanțe într-o id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Afirmațiile](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) la care vă puteți aștepta în tokenuri ID și simboluri de acces emise de AZURE AD B2C
- [Referință pentru revendicările tokenului SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
