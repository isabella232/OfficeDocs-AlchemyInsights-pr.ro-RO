---
title: Configurare LDAP
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090424"
---
# <a name="configure-ldap"></a>Configurare LDAP

Pentru a configura LDAP, faceți următoarele:

1. Verificați starea domeniului dvs. pe [portalul Azure.](https://aka.ms/aadds-health)
1. Asigurați-vă că este disponibil un abonament Azure AD valid și că a fost activat Azure AD Domain Services.
1. Certificatul necesar pentru a activa LDAP securizat trebuie să fie obținut de la o autoritate de certificare publică de încredere sau să fie un certificat auto-semnat.
1. Asigurați-vă că certificatul respectă regulile [necesare.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Certificat nevalid**
1. Pentru a reînnoi un certificat, urmați pașii pentru a crea un nou certificat și a reîncărca: [Configurați LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Pentru a rezolva problema cunoscută cu avertizările LDAP securizate din Serviciile de domeniu Azure Active directory, consultați [Rezolvarea avertizărilor LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
