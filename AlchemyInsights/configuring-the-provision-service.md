---
title: Configurarea serviciului de furnizare a accesului
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033290"
---
# <a name="configuring-the-provision-service"></a>Configurarea serviciului de furnizare a accesului

Pentru ca asigurarea accesului automat al utilizatorilor să lucreze, Azure AD necesită acreditări valide care îi permit să se conecteze la API Workday Web Services. În continuare, butonul Testare conexiune din ziua de lucru la aplicația Asigurare acces pentru utilizatorii AD validează și dacă se poate conecta la Agentul de furnizare a accesului Azure AD Conectare asociat cu domeniul AD.

Dacă portalul Azure returnează o eroare la salvarea acreditărilor, urmați pașii recomandați de mai jos:

1. Confirmați că ați configurat Contul de utilizator pentru integrarea cu workday, după cum se precizează în secțiunea de tutorial Configurarea utilizatorului [sistemului de integrare în Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Confirmați că Serviciul agent de Conectare Azure AD Conectare este activat și rulează pe serverul dvs. Windows local, utilizând Consola de gestionare a serviciilor. De asemenea, puteți verifica starea agentului în portalul Azure, făcând clic pe butonul Vizualizare agenți locali.
3. Asigurați-vă că introduceți valoarea pentru câmpul "Nume utilizator zi lucrătoare" utilizând formatul username@workday-numele entității găzduite. Dacă lipsește numele de entitate găzduită al zilei de lucru, autentificarea pentru ziua de lucru nu reușește.
4. Dacă configurați integrarea cu entitatea găzduită de implementare Workday, rețineți orele de neconfigurate ale entității găzduite pentru zilele lucrătoare. Ziua de lucru a programat o perioadă de neimplementarea entităților găzduite în weekend (de obicei, de vineri seara până sâmbătă dimineața) și erorile de conectivitate din timpul acestei ferestre de neconectare este o problemă cunoscută care se rezolvă automat imediat ce entitățile găzduite de implementare revin online.
5. În cazuri rare, este posibil să vedeți această eroare și dacă parola utilizatorului de sistem de integrare s-a modificat din cauza reîmprospătării entității găzduite sau dacă contul este în starea blocat sau expirat. Verificați starea utilizatorului Sistem de integrare cu administratorul dvs. de zi de lucru.

Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea automată a accesului, consultați Tutorial: Configurarea zilei de lucru pentru asigurarea automată [a accesului utilizatorilor.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
