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
# <a name="configuring-the-provision-service"></a><span data-ttu-id="526f0-102">Configurarea serviciului de furnizare</span><span class="sxs-lookup"><span data-stu-id="526f0-102">Configuring the Provision service</span></span>

<span data-ttu-id="526f0-103">Pentru ca utilizatorul să aibă acces automat la serviciu, Azure AD necesită acreditări valide care îi permit să se conecteze la ziua de lucru Web Services API.</span><span class="sxs-lookup"><span data-stu-id="526f0-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="526f0-104">Mai departe, butonul de test de conexiune de la data de lucru la aplicația de asigurare a accesului pentru utilizatori AD validează, de asemenea, dacă se poate conecta la agentul Azure AD Connect Provisioning asociat domeniului de publicitate.</span><span class="sxs-lookup"><span data-stu-id="526f0-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="526f0-105">Dacă portalul Azure returnează o eroare la salvarea acreditărilor, urmați pașii de mai jos:</span><span class="sxs-lookup"><span data-stu-id="526f0-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="526f0-106">Confirmați că ați configurat contul de utilizator al sistemului de integrare lucrătoare, așa cum se indică în secțiunea tutorial, [configurați utilizatorul sistemului de integrare în ziua de](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)lucru.</span><span class="sxs-lookup"><span data-stu-id="526f0-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="526f0-107">Confirmați că serviciul de agent de furnizare Azure AD Connect este în funcțiune pe serverul Windows local, utilizând consola de gestionare a serviciilor.</span><span class="sxs-lookup"><span data-stu-id="526f0-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="526f0-108">De asemenea, puteți să verificați starea agentului în portalul Azure, făcând clic pe butonul Vizualizare agenți locali.</span><span class="sxs-lookup"><span data-stu-id="526f0-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="526f0-109">Asigurați-vă că introduceți valoarea pentru câmpul "zi de lucru nume", utilizând formatul username@workday-entitatea găzduită.</span><span class="sxs-lookup"><span data-stu-id="526f0-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="526f0-110">Dacă numele de zi de lucru-entitatea găzduită lipsește, autentificarea zilei de lucru nu reușește.</span><span class="sxs-lookup"><span data-stu-id="526f0-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="526f0-111">În cazul în care configurați integrarea cu entitatea găzduită de execuție de zile lucrătoare, notați orele de downtime programate ale entității găzduite lucrătoare.</span><span class="sxs-lookup"><span data-stu-id="526f0-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="526f0-112">Ziua de lucru a programat timp pentru entitățile găzduite de implementare în week-end (de obicei, de vineri seara până sâmbătă dimineață) și erorile de conectivitate din această fereastră de nefuncționare este o problemă cunoscută care se rezolvă automat imediat ce entitățile găzduite de implementare sunt din nou online.</span><span class="sxs-lookup"><span data-stu-id="526f0-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="526f0-113">În cazuri rare, este posibil să vedeți această eroare și dacă parola utilizatorului sistemului de integrare s-a modificat din cauza reîmprospătării entității găzduite sau dacă contul este în stare blocată sau expirată.</span><span class="sxs-lookup"><span data-stu-id="526f0-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="526f0-114">Vă rugăm să verificați starea utilizatorului de sistem de integrare cu administratorul zilei de lucru.</span><span class="sxs-lookup"><span data-stu-id="526f0-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="526f0-115">Pentru mai multe detalii despre configurarea zilei de lucru pentru asigurarea accesului automat, consultați [Tutorial: Configurarea zilei de lucru pentru asigurarea accesului automat la utilizatori](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="526f0-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
