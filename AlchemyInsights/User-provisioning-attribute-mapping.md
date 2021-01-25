---
title: Maparea atributului de asigurare a accesului utilizatorilor
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949893"
---
# <a name="user-provisioning-attribute-mapping"></a>Maparea atributului de asigurare a accesului utilizatorilor

1. Pentru a depana problemele cunoscute de mapare a atributelor, consultați [asocierile atributurilor](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) oferă suport pentru asigurarea accesului utilizatorilor la aplicații SaaS de la terți, cum ar fi Salesforce, G Suite și altele. Dacă activați asigurarea accesului utilizatorilor pentru o aplicație SaaS de la terți, portalul Azure controlează valorile sale de atribut prin mapări de atribute. Pentru a afla cum să particularizați mapările de atribute implicite, consultați [Particularizarea atributului de asigurare a accesului utilizatorilor-mapări pentru aplicațiile SaaS din Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Pentru a afla mai multe despre asigurarea accesului utilizatorilor de aplicații SaaS, consultați [ce este asigurarea accesului utilizatorilor automat SaaS App în AZURE AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Atunci când particularizați mapări de atribute pentru asigurarea accesului utilizatorilor, este posibil să descoperiți că atributul pe care doriți să îl mapați nu apare în lista de atribute sursă. [Sincronizarea unui atribut din Active Directory local la AZURE AD pentru asigurarea accesului la un](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) articol de aplicație vă arată cum să adăugați atributul lipsă, dacă îl sincronizați de la reclama locală la Azure AD.
