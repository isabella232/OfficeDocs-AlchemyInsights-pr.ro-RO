---
title: Configurarea serviciului de furnizare
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484041"
---
# <a name="configuring-the-provision-service"></a>Configurarea serviciului de furnizare

Pentru ca utilizatorul să aibă acces automat la serviciu, Azure AD necesită acreditări valide care îi permit să se conecteze la ziua de lucru Web Services API. Mai departe, butonul de test de conexiune de la data de lucru la aplicația de asigurare a accesului pentru utilizatori AD validează, de asemenea, dacă se poate conecta la agentul Azure AD Connect Provisioning asociat domeniului de publicitate.

Dacă portalul Azure returnează o eroare la salvarea acreditărilor, urmați pașii de mai jos:

1. Confirmați că ați configurat contul de utilizator al sistemului de integrare lucrătoare, așa cum se indică în secțiunea tutorial, [configurați utilizatorul sistemului de integrare în ziua de](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)lucru.
2. Confirmați că serviciul de agent de furnizare Azure AD Connect este în funcțiune pe serverul Windows local, utilizând consola de gestionare a serviciilor. De asemenea, puteți să verificați starea agentului în portalul Azure, făcând clic pe butonul Vizualizare agenți locali.
3. Asigurați-vă că introduceți valoarea pentru câmpul "zi de lucru nume", utilizând formatul username@workday-entitatea găzduită. Dacă numele de zi de lucru-entitatea găzduită lipsește, autentificarea zilei de lucru nu reușește.
4. În cazul în care configurați integrarea cu entitatea găzduită de execuție de zile lucrătoare, notați orele de downtime programate ale entității găzduite lucrătoare. Ziua de lucru a programat timp pentru entitățile găzduite de implementare în week-end (de obicei, de vineri seara până sâmbătă dimineață) și erorile de conectivitate din această fereastră de nefuncționare este o problemă cunoscută care se rezolvă automat imediat ce entitățile găzduite de implementare sunt din nou online.
5. În cazuri rare, este posibil să vedeți această eroare și dacă parola utilizatorului sistemului de integrare s-a modificat din cauza reîmprospătării entității găzduite sau dacă contul este în stare blocată sau expirată. Vă rugăm să verificați starea utilizatorului de sistem de integrare cu administratorul zilei de lucru.

Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea accesului automat, consultați [Tutorial: Configurarea zilei de lucru pentru asigurarea accesului automat la utilizatori](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
