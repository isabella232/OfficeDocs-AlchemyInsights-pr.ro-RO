---
title: Configurarea și particularizarea aplicațiilor
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063663"
---
# <a name="configure-and-customize-applications"></a>Configurarea și particularizarea aplicațiilor

**Configurarea aplicațiilor**

1. [Pornire rapidă: Configurarea proprietăților pentru o aplicație din entitatea găzduită Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vă arată cum să configurați unele dintre proprietățile unei aplicații.
2. Pentru a contribui la integrarea aplicațiilor cu Azure Active Directory, am dezvoltat [o colecție de tutoriale](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) care vă ghidează prin configurare.
3. [Cum se configurează o aplicație proxy de aplicație](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) vă ajută să înțelegeți cum să configurați o aplicație proxy de aplicație din Azure AD pentru a expune aplicațiile locale în cloud.
4. [Descărcați PingAccess și configurați aplicația](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): urmați instrucțiunile din *Configurarea PINGACCESS pentru Azure AD pentru a proteja aplicațiile* publicate utilizând Microsoft Azure AD Application proxy pe site-ul web ping Identity și descărcați cea mai recentă versiune de PingAccess.

**Erori de aplicație configurate incorect (AADSTS650056)**

1. Asigurați-vă că Accesați aplicația din adresa de conectare furnizată de proprietarul aplicației. Altfel înțeles, conectați-vă la aplicație prin procesul său normal. În majoritatea cazurilor, aceasta se va rezolva automat în mod natural. Dacă nu face acest lucru, această publicare poate contribui la depanarea și rezolvarea acestuia.
2. **Dacă organizația dumneavoastră deține aplicația** (adică înregistrarea aplicației se află în organizația dvs.):
    - La minimum, vă recomandăm să `User.Read` `openid` Adăugați permisiunea sau delegatul din **Microsoft Graph** .
    - Asigurați-vă că aplicația și toate permisiunile sale sunt consimțite. Puteți verifica acest lucru consultând coloana **stare** a înregistrării de aplicație din **permisiunile API**.
    - În unele scenarii, aplicația poate fi de la terți, însă poate fi înregistrată în organizația dvs. Confirmați dacă această aplicație este listată în înregistrările aplicațiilor (nu în aplicațiile Enterprise).
    - Dacă continuați să vedeți acest mesaj de eroare. Atunci poate fi necesar să creați URL-ul de consimțământ descris în **Pasul 4**.
3. **Dacă organizația nu este proprietarul aplicației și o folosește ca aplicație de la terți**:
    - Dacă sunteți administratorul global/firmă, ar trebui să vedeți ecranul consimțământ. Asigurați-vă că bifați caseta pentru **"consimțământ în numele organizației"**.
    - Dacă nu vedeți ecranul de consimțământ, ștergeți aplicația Enterprise și încercați din nou.
    - Dacă continuați să vedeți acest mesaj de eroare. Atunci poate fi necesar să creați URL-ul de consimțământ descris în **Pasul 4**.
4. **Creați manual adresa URL de aprobare de utilizat**: dacă aplicația este proiectată pentru a accesa o anumită resursă, este posibil să nu reușiți să utilizați butoanele de consimțământ din portalul Azure, va trebui să generați manual propriul URL de consimțământ și să îl utilizați.
    - Va trebui să obțineți și de la `{App-Id}` `{App-Uri-Id}` proprietarul aplicației. `{Tenant-Id}` va fi identificatorul entității găzduite. Aceasta va fi fie `yourdomain.onmicrosoft.com` sau ID-ul de director.
    - Dacă aplicația se accesează singură pentru resursă, atunci `{App-Id}` și `{App-Uri-Id}` va fi aceeași.
5. Pentru mai multe informații, consultați [probleme la conectarea la aplicațiile configurate pentru sign-on unic bazat pe SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Particularizarea aplicațiilor**

- [Adăugarea de branding la pagina de conectare Azure Active Directory a Organizației](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) dvs., utilizați sigla organizației și schemele de culori particularizate pentru a oferi un aspect consistent și paginilor de conectare Azure Active Directory (Azure AD).
- [Adăugați numele de domeniu particularizat utilizând portalul Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) -fiecare nouă entitate găzduită Azure AD este livrată cu un nume de domeniu inițial. Nu puteți să modificați sau să ștergeți numele de domeniu inițial, dar puteți să adăugați numele organizației. Adăugarea numelor de domenii particularizate vă ajută să creați nume de utilizator care sunt familiare pentru utilizatorii dvs.
