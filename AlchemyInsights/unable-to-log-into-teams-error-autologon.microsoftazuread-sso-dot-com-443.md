---
title: Nu vă puteți conecta la Teams din cauza erorii autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932034"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="59d6c-102">Nu vă puteți conecta la Teams din cauza erorii autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="59d6c-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="59d6c-103">Dacă Seamless SSO este activat ca autentificare O365, poate fi necesar ca adresa URL "autologon.microsoftazuread-sso.com" să fie adăugată la Site-uri Intranet.</span><span class="sxs-lookup"><span data-stu-id="59d6c-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="59d6c-104">Dacă s-a adăugat anterior la Site-uri de Încredere și Seamless SSO este în utilizare, acesta ar trebui eliminat din Site-uri de Încredere.</span><span class="sxs-lookup"><span data-stu-id="59d6c-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="59d6c-105">Vă rugăm să consultați [Lista de Verificare pentru Depanarea Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="59d6c-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="59d6c-106">Urmați acești pași pentru a adăuga o adresă URL în lista de Site-uri Intranet:</span><span class="sxs-lookup"><span data-stu-id="59d6c-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="59d6c-107">Deschideți Internet Explorer făcând clic pe butonul **Start**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="59d6c-108">În caseta de căutare, tastați Internet Explorer, apoi, în lista de rezultate, faceți clic pe **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="59d6c-109">Faceți clic pe **Instrumente**, apoi faceți clic pe **Opțiuni Internet**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="59d6c-110">Faceți clic pe fila **Securitate**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="59d6c-111">Acum faceți clic pe **site-uri Intranet Locale** apoi faceți clic pe butonul **site-uri**, apoi butonul de **Avansate**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="59d6c-112">Introduceți URL-ul site-ului web și faceți clic pe **Adăugare**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="59d6c-113">Când ați terminat, faceți clic pe **Închidere**.</span><span class="sxs-lookup"><span data-stu-id="59d6c-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="59d6c-114">Pentru mai multe informații, consultați [Documentație pentru implementarea Seamless SSO pentru O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (include procese bazate pe politici pentru a adăuga un URL la Site-uri Intranet la pasul 3).</span><span class="sxs-lookup"><span data-stu-id="59d6c-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
