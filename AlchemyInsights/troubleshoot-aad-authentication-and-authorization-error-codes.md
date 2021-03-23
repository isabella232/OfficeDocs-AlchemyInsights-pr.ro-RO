---
title: Depanarea codurilor de eroare pentru autentificarea și autorizarea Azure AD (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037836"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Depanarea codurilor de eroare pentru autentificarea și autorizarea Azure AD (AADSTS)

Pentru a rezolva codurile de eroare de autentificare și autorizare din AAD (AADSTS), efectuați următorii pași recomandați:

1. **Manipularea codurilor de eroare în aplicație**

- **Spec. OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 furnizează instrucțiuni despre cum să gestionați erorile în timpul autentificării utilizând porțiunea de eroare a răspunsului de eroare.

    - **Eroare**: un șir de cod de eroare care poate fi utilizat pentru a clasifica tipurile de erori care apar și ar trebui să fie utilizate pentru a reacționa la erori.
    - Câmpul de **Eroare** are mai multe valori posibile-revizuiți linkurile de documentație protocol și specificatiile OAuth 2,0 pentru mai multe informații despre anumite erori și cum să reacționați la acestea.

- Iată un exemplu de răspuns de eroare:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Informații despre codul de eroare de căutare curent**

- Codurile de eroare și mesajele se pot modifica. Pentru cele mai recente informații, consultați https://login.microsoftonline.com/error pagina pentru a găsi descrieri de erori AADSTS, remedieri și câteva soluții sugerate.
- De asemenea, puteți să căutați și să depanați [codurile de eroare AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listate în [codurile de eroare Azure AD Authentication and autorizare](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Obțineți ajutor**

- [Opțiuni de asistență și ajutor pentru dezvoltatori](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -dacă aveți nevoie de un răspuns la o întrebare sau ajutor pentru a rezolva o problemă care nu este acoperită de documentația noastră, poate fi timpul să contactați experții pentru ajutor. Acest articol oferă mai multe sugestii pentru a primi răspunsuri la întrebări în timp ce Dezvoltați aplicații care se integrează cu platforma de identitate Microsoft.








