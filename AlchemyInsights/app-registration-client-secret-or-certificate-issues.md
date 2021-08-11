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
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951505"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Probleme secrete ale clientului de înregistrare a aplicațiilor sau ale certificatelor

Clientul aplicației expiră secret?

Indiferent cum a fost creată aplicația înregistrată, fie prin procesul de înregistrare standard din portalul de înregistrare a aplicațiilor, fie dacă entitatea principală de serviciu a fost creată în entitatea dvs. găzduită folosind consimțământul aplicației, va trebui creat un nou Secret client înainte de expirarea acestuia curent și actualizat în codul aplicației asociate. Perioada maximă de validitate este de 2 ani. Ca memento, valoarea secretă trebuie înregistrată, deoarece nu va mai fi vizibilă după ce părăsiți pagina de înregistrări a aplicațiilor din portal. Pentru mai multe informații, [consultați Pornire rapidă: Înregistrați](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) o aplicație în Serviciu de identitate Microsoft și Cele mai bune practici pentru această [Serviciu de identitate Microsoft](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Pentru a afla mai multe, [consultați Crearea unei aplicații Azure AD & principal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)de serviciu în portal - Serviciu de identitate Microsoft .
