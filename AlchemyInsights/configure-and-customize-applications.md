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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045000"
---
# <a name="configure-and-customize-applications"></a>Configurarea și particularizarea aplicațiilor

**Configurarea aplicațiilor**

1. Pornire rapidă: Configurarea proprietăților pentru o aplicație din entitatea găzduită [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vă arată cum să configurați unele proprietăți pentru o aplicație.
2. Pentru a contribui la integrarea aplicațiilor cu Azure Active Directory, am dezvoltat o colecție de [tutoriale care](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) vă ajută să faceți o configurare.
3. [Modul de configurare a unei aplicații Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) aplicație vă ajută să înțelegeți cum să configurați o aplicație Proxy de aplicație în cadrul Azure AD pentru a expune aplicațiile dvs. local în cloud.
4. [Descărcați PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)și configurați aplicația: Urmați instrucțiunile din Configurarea *PingAccess* pentru Azure AD pentru Microsoft Azure AD proteja aplicațiile publicate utilizând un proxy de aplicație pe site-ul web Ping Identity și descărcați cea mai recentă versiune de PingAccess.

**Erori de aplicație de configurare greșită (AADSTS650056)**

1. Asigurați-vă că accesați aplicația de la adresa de conectare furnizată de proprietarul aplicației. În caz contrar, conectați-vă la aplicație prin procesul normal al acesteia. În majoritatea cazurilor, aceasta se va rezolva automat în mod natural. Dacă nu le rezolvă, această postare vă poate ajuta să o depanați și să o rezolvați.
2. **Dacă organizația dvs. deține aplicația (ceea ce** înseamnă că înregistrarea aplicației se află în organizația dvs.):
    - Se recomandă cel puțin permisiunea `User.Read` `openid` delegată de la **Microsoft Graph** adăuga.
    - Asigurați-vă că aplicația și toate permisiunile sale sunt de acord. Puteți verifica acest lucru privind coloana **Stare din înregistrarea** aplicației din Permisiuni **API.**
    - În unele scenarii, aplicația poate fi terță, însă poate fi înregistrată în organizația dvs. Confirmați dacă această aplicație este listată în înregistrările de aplicații (nu în aplicațiile Enterprise).
    - Dacă vedeți în continuare acest mesaj de eroare. Apoi poate fi necesar să construiți adresa URL de consimțământ **descrisă în pasul 4.**
3. **Dacă organizația dvs. nu este proprietarul aplicației și o utilizați ca aplicație terță:**
    - Dacă sunteți administratorul global/al firmei, ar trebui să vedeți ecranul de consimțământ. Asigurați-vă că bifați caseta **"Consimțământul în numele organizației dvs.".**
    - Dacă nu vedeți ecranul de consimțământ, ștergeți aplicația Enterprise și încercați din nou.
    - Dacă vedeți în continuare acest mesaj de eroare. Apoi poate fi necesar să construiți adresa URL de consimțământ **descrisă în pasul 4.**
4. Creați manual adresa **URL** de consimțământ pentru utilizare: Dacă aplicația este proiectată să acceseze o anumită resursă, este posibil să nu puteți utiliza butoanele de consimțământ din portalul Azure, va trebui să generați manual propriul URL de consimțământ și să îl utilizați.
    - Va trebui să obțineți și `{App-Id}` de la `{App-Uri-Id}` proprietarul aplicației. `{Tenant-Id}` va fi identificatorul entității găzduite. Acesta va fi sau `yourdomain.onmicrosoft.com` ID-ul dvs. de director.
    - Dacă aplicația se accesează singură pentru resursă, atunci `{App-Id}` și va fi la `{App-Uri-Id}` fel.
5. Pentru mai multe informații, [consultați Probleme la conectarea la aplicațiile configurate de sign-on unic bazate pe SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Customize Applications**

- Adăugarea unui [branding](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) la pagina de conectare Azure Active Directory a organizației: utilizați sigla organizației și schemele de culori particularizate pentru a oferi un aspect unitar paginilor de conectare Azure Active Directory (Azure AD).
- [Adăugați numele de domeniu particularizat utilizând portalul Azure Active Directory- Fiecare](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) entitate găzduită Azure AD nouă are un nume de domeniu inițial. Nu puteți să modificați sau să ștergeți numele de domeniu inițial, dar puteți adăuga numele organizației dvs. Adăugarea numelor de domeniu particularizate vă ajută să creați nume de utilizator familiare utilizatorilor dvs.
