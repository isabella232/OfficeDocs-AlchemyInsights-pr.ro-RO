---
title: Probleme secrete ale clientului de înregistrare a aplicațiilor sau ale certificatelor
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405335"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Probleme secrete ale clientului de înregistrare a aplicațiilor sau ale certificatelor

Clientul aplicației expiră secret?

Indiferent cum a fost creată aplicația înregistrată, fie prin procesul de înregistrare standard din portalul de înregistrare a aplicațiilor, fie dacă entitatea principală de serviciu a fost creată în entitatea dvs. găzduită folosind consimțământul aplicației, va trebui creat un nou Secret client înainte de expirarea acestuia curent și actualizat în codul aplicației asociate. Perioada maximă de validitate este de 2 ani. Ca memento, valoarea secretă trebuie înregistrată, deoarece nu va mai fi vizibilă după ce părăsiți pagina de înregistrări a aplicațiilor din portal. Pentru mai multe informații, consultați [Pornire rapidă: Înregistrați o](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplicație pe platforma de identitate Microsoft și Cele mai bune practici pentru platforma de identitate [Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Pentru a afla mai multe, consultați Crearea unui cont principal de & de aplicație [Azure AD în portalul - platforma de identitate Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
