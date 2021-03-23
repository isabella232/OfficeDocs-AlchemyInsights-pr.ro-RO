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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="0a120-102">Depanarea codurilor de eroare pentru autentificarea și autorizarea Azure AD (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="0a120-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="0a120-103">Pentru a rezolva codurile de eroare de autentificare și autorizare din AAD (AADSTS), efectuați următorii pași recomandați:</span><span class="sxs-lookup"><span data-stu-id="0a120-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="0a120-104">**Manipularea codurilor de eroare în aplicație**</span><span class="sxs-lookup"><span data-stu-id="0a120-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="0a120-105">**Spec. OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 furnizează instrucțiuni despre cum să gestionați erorile în timpul autentificării utilizând porțiunea de eroare a răspunsului de eroare.</span><span class="sxs-lookup"><span data-stu-id="0a120-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="0a120-106">**Eroare**: un șir de cod de eroare care poate fi utilizat pentru a clasifica tipurile de erori care apar și ar trebui să fie utilizate pentru a reacționa la erori.</span><span class="sxs-lookup"><span data-stu-id="0a120-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="0a120-107">Câmpul de **Eroare** are mai multe valori posibile-revizuiți linkurile de documentație protocol și specificatiile OAuth 2,0 pentru mai multe informații despre anumite erori și cum să reacționați la acestea.</span><span class="sxs-lookup"><span data-stu-id="0a120-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="0a120-108">Iată un exemplu de răspuns de eroare:</span><span class="sxs-lookup"><span data-stu-id="0a120-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="0a120-109">**Informații despre codul de eroare de căutare curent**</span><span class="sxs-lookup"><span data-stu-id="0a120-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="0a120-110">Codurile de eroare și mesajele se pot modifica.</span><span class="sxs-lookup"><span data-stu-id="0a120-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="0a120-111">Pentru cele mai recente informații, consultați https://login.microsoftonline.com/error pagina pentru a găsi descrieri de erori AADSTS, remedieri și câteva soluții sugerate.</span><span class="sxs-lookup"><span data-stu-id="0a120-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="0a120-112">De asemenea, puteți să căutați și să depanați [codurile de eroare AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listate în [codurile de eroare Azure AD Authentication and autorizare](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="0a120-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="0a120-113">**Obțineți ajutor**</span><span class="sxs-lookup"><span data-stu-id="0a120-113">**Get Help**</span></span>

- <span data-ttu-id="0a120-114">[Opțiuni de asistență și ajutor pentru dezvoltatori](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) -dacă aveți nevoie de un răspuns la o întrebare sau ajutor pentru a rezolva o problemă care nu este acoperită de documentația noastră, poate fi timpul să contactați experții pentru ajutor.</span><span class="sxs-lookup"><span data-stu-id="0a120-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="0a120-115">Acest articol oferă mai multe sugestii pentru a primi răspunsuri la întrebări în timp ce Dezvoltați aplicații care se integrează cu platforma de identitate Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0a120-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








