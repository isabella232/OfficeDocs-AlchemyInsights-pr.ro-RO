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
# <a name="configure-ldap"></a>Configurarea LDAP

Pentru a configura LDAP, procedați astfel:

1. Verificați sănătatea domeniului în [portalul Azure](https://aka.ms/aadds-health).
1. Asigurați-vă că este disponibil un abonament Azure AD corect și că serviciile de domeniu Azure AD au fost activate.
1. Certificatul necesar pentru a activa LDAP securizat trebuie să fie obținut de la o autoritate de certificare publică de încredere sau să fie un certificat cu semnătură automată.
1. Asigurați-vă că certificatul urmează [instrucțiunile](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)necesare.

**Certificat nevalid**
1. Pentru a reînnoi un certificat, urmați pașii pentru a crea un certificat nou și a reîncărca: [configurați LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Pentru a rezolva problema cunoscută cu avertizările LDAP securizate în serviciile de domeniu Azure Active Directory, consultați [rezolvarea alertelor LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
