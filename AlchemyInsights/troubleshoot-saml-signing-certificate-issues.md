---
title: Depanarea problemelor de certificat de semnare SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694447"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Depanarea problemelor de certificat de semnare SAML

Pentru a rezolva problema de certificat de semnare SAML, efectuați următorii pași recomandate:

1. Atunci când adăugați o aplicație de întreprindere care acceptă SSO, Azure va genera un certificat denumit certificat de [semnare SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Acest certificat are o dată de expirare de 3 ani. Pentru a modifica data de expirare a certificatului, consultați [Particularizarea datei de expirare pentru certificatul de federalizare și răsturnarea acestuia la un certificat nou](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure va utiliza acest certificat pentru a semna token-ul SAML solicitat de aplicație și a-l trimite la aplicație pentru o SSO reușită. Pentru ca aceasta să se termine, descărcați certificatul din portalul Azure și trimiteți-l la furnizorul aplicației pentru a finaliza procesul SSO.

După ce acest proces finalizează aplicația, va avea încredere în acest certificat și toate jetoanele SAML semnate de acest certificat vor fi acceptate de aplicație.

3. Dacă acest certificat expiră, creați un certificat nou, actualizați-l la furnizorul aplicației, apoi faceți-l activ în partea Azure. Pentru mai multe informații, consultați [reînnoirea unui certificat care va expira în curând](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Dacă certificatul expiră, utilizatorul nu va fi blocat.

4. [Adăugați o adresă de e-mail pentru ca notificările](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) să fie primite înainte ca certificatul curent să expire.

> [!NOTE]
> Pasul 4 este unul opțional.

5. Modificați opțiunile de semnare a certificatului SAML ale unei aplicații și algoritmul de semnare a certificatului. Pentru mai multe informații, consultați [modificarea opțiunilor de semnare a certificatului și a algoritmului de semnare](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

