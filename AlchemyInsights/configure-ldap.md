---
title: Configurarea LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885575"
---
# <a name="configure-ldap"></a><span data-ttu-id="3728d-102">Configurarea LDAP</span><span class="sxs-lookup"><span data-stu-id="3728d-102">Configure LDAP</span></span>

<span data-ttu-id="3728d-103">Pentru a configura LDAP, procedați astfel:</span><span class="sxs-lookup"><span data-stu-id="3728d-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="3728d-104">Verificați sănătatea domeniului în [portalul Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="3728d-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="3728d-105">Asigurați-vă că este disponibil un abonament Azure AD corect și că serviciile de domeniu Azure AD au fost activate.</span><span class="sxs-lookup"><span data-stu-id="3728d-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="3728d-106">Certificatul necesar pentru a activa LDAP securizat trebuie să fie obținut de la o autoritate de certificare publică de încredere sau să fie un certificat cu semnătură automată.</span><span class="sxs-lookup"><span data-stu-id="3728d-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="3728d-107">Asigurați-vă că certificatul urmează [instrucțiunile](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)necesare.</span><span class="sxs-lookup"><span data-stu-id="3728d-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="3728d-108">**Certificat nevalid**</span><span class="sxs-lookup"><span data-stu-id="3728d-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="3728d-109">Pentru a reînnoi un certificat, urmați pașii pentru a crea un certificat nou și a reîncărca: [configurați LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3728d-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="3728d-110">Pentru a rezolva problema cunoscută cu avertizările LDAP securizate în serviciile de domeniu Azure Active Directory, consultați [rezolvarea alertelor LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3728d-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
