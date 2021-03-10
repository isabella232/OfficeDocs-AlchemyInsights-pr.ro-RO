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
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="b4271-102">Depanarea problemelor de certificat de semnare SAML</span><span class="sxs-lookup"><span data-stu-id="b4271-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="b4271-103">Pentru a rezolva problema de certificat de semnare SAML, efectuați următorii pași recomandate:</span><span class="sxs-lookup"><span data-stu-id="b4271-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="b4271-104">Atunci când adăugați o aplicație de întreprindere care acceptă SSO, Azure va genera un certificat denumit certificat de [semnare SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="b4271-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="b4271-105">Acest certificat are o dată de expirare de 3 ani.</span><span class="sxs-lookup"><span data-stu-id="b4271-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="b4271-106">Pentru a modifica data de expirare a certificatului, consultați [Particularizarea datei de expirare pentru certificatul de federalizare și răsturnarea acestuia la un certificat nou](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="b4271-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="b4271-107">Azure va utiliza acest certificat pentru a semna token-ul SAML solicitat de aplicație și a-l trimite la aplicație pentru o SSO reușită.</span><span class="sxs-lookup"><span data-stu-id="b4271-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="b4271-108">Pentru ca aceasta să se termine, descărcați certificatul din portalul Azure și trimiteți-l la furnizorul aplicației pentru a finaliza procesul SSO.</span><span class="sxs-lookup"><span data-stu-id="b4271-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="b4271-109">După ce acest proces finalizează aplicația, va avea încredere în acest certificat și toate jetoanele SAML semnate de acest certificat vor fi acceptate de aplicație.</span><span class="sxs-lookup"><span data-stu-id="b4271-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="b4271-110">Dacă acest certificat expiră, creați un certificat nou, actualizați-l la furnizorul aplicației, apoi faceți-l activ în partea Azure.</span><span class="sxs-lookup"><span data-stu-id="b4271-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="b4271-111">Pentru mai multe informații, consultați [reînnoirea unui certificat care va expira în curând](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="b4271-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="b4271-112">Dacă certificatul expiră, utilizatorul nu va fi blocat.</span><span class="sxs-lookup"><span data-stu-id="b4271-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="b4271-113">[Adăugați o adresă de e-mail pentru ca notificările](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) să fie primite înainte ca certificatul curent să expire.</span><span class="sxs-lookup"><span data-stu-id="b4271-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="b4271-114">Pasul 4 este unul opțional.</span><span class="sxs-lookup"><span data-stu-id="b4271-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="b4271-115">Modificați opțiunile de semnare a certificatului SAML ale unei aplicații și algoritmul de semnare a certificatului.</span><span class="sxs-lookup"><span data-stu-id="b4271-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="b4271-116">Pentru mai multe informații, consultați [modificarea opțiunilor de semnare a certificatului și a algoritmului de semnare](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="b4271-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

