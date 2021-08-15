---
title: Nu vă puteți conecta la Teams din cauza erorii autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038412"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nu vă puteți conecta la Teams din cauza erorii autologon.microsoftazuread-sso dot com:443

Dacă Seamless SSO este activat ca autentificare O365, poate fi necesar ca adresa URL "autologon.microsoftazuread-sso.com" să fie adăugată la Site-uri Intranet.  Dacă s-a adăugat anterior la Site-uri de Încredere și Seamless SSO este în utilizare, acesta ar trebui eliminat din Site-uri de Încredere.

Vă rugăm să consultați [Lista de Verificare pentru Depanarea Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Urmați acești pași pentru a adăuga o adresă URL în lista de Site-uri Intranet:

1. Deschideți Internet Explorer făcând clic pe butonul **Start**. În caseta de căutare, tastați Internet Explorer, apoi, în lista de rezultate, faceți clic pe **Internet Explorer**.
2. Faceți clic pe **Instrumente**, apoi faceți clic pe **Opțiuni Internet**.
3. Faceți clic pe fila **Securitate**.
4. Acum faceți clic pe **site-uri Intranet Locale** apoi faceți clic pe butonul **site-uri**, apoi butonul de **Avansate**.
5. Introduceți URL-ul site-ului web și faceți clic pe **Adăugare**.
6. Când ați terminat, faceți clic pe **Închidere**.

Pentru mai multe informații, consultați [Documentație pentru implementarea Seamless SSO pentru O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (include procese bazate pe politici pentru a adăuga un URL la Site-uri Intranet la pasul 3).
