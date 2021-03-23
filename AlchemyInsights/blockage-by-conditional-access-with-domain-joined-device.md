---
title: Sunt blocat de acces condiționat cu un dispozitiv asociat domeniului
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038100"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="c43ce-102">Sunt blocat de acces condiționat cu un dispozitiv asociat domeniului</span><span class="sxs-lookup"><span data-stu-id="c43ce-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="c43ce-103">**Instrumente foarte recomandate**</span><span class="sxs-lookup"><span data-stu-id="c43ce-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="c43ce-104">Instrument de depanare a [înregistrărilor dispozitivelor](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -instrumentul care ajută la depanarea problemelor cele mai comune de înregistrare a dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="c43ce-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="c43ce-105">[Test de conectivitate pentru înregistrarea dispozitivului](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -scriptul care vă ajută să vă asigurați că un dispozitiv poate accesa punctele finale de înregistrare a dispozitivelor de sub contul de sistem.</span><span class="sxs-lookup"><span data-stu-id="c43ce-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="c43ce-106">[Script de curățire a dispozitivului AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -scenariul care vă permite să căutați și să gestionați dispozitivele vechi în mediul dvs.</span><span class="sxs-lookup"><span data-stu-id="c43ce-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="c43ce-107">Iată câteva motive comune pentru care accesul condiționat este posibil să nu reușească un dispozitiv care s-a alăturat unui domeniu (hibrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c43ce-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="c43ce-108">Nu **există niciun PRT-ul AZURE ad pe dispozitiv** -trebuie să vă asigurați că dispozitivul are simbolul de reîmprospătare primară Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="c43ce-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="c43ce-109">Pentru mai multe informații despre PRT, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="c43ce-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="c43ce-110">Pentru a verifica dacă aveți Azure AD PRT, puteți să executați `dsregcmd/status` comanda pe dispozitiv și să verificați dacă "AzureAdPrt" este egal cu "Da".</span><span class="sxs-lookup"><span data-stu-id="c43ce-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="c43ce-111">Dacă "AzureAdPrt" este "nu", verificați următoarele:</span><span class="sxs-lookup"><span data-stu-id="c43ce-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="c43ce-112">**Indiferent dacă aveți un mediu federativ cu AD FS și este inaccesibil din rețelele de domiciliu ale utilizatorilor**: în acest caz, asigurați-vă că punctele finale "usernamemixed" sunt accesibile de la extranet.</span><span class="sxs-lookup"><span data-stu-id="c43ce-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="c43ce-113">Dacă AD FS se află în spatele unei rețele VPN, asigurați-vă că utilizatorii se conectează la VPN și se reconectează la dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="c43ce-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="c43ce-114">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="c43ce-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="c43ce-115">**Dacă TPM-ul dispozitivului este defect și, prin urmare, nu poate autentifica dispozitivul**: bifați "TPM. msc" pentru a vedea dacă starea TPM este "gata".</span><span class="sxs-lookup"><span data-stu-id="c43ce-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="c43ce-116">Dacă nu, rulare `dsregcmd/leave` și permiteți reasocierea dispozitivului la AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="c43ce-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="c43ce-117">Apoi încercați din nou.</span><span class="sxs-lookup"><span data-stu-id="c43ce-117">Then, try again.</span></span> <span data-ttu-id="c43ce-118">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="c43ce-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="c43ce-119">**Utilizați un furnizor de identitate terț, care nu acceptă protocolul WS-Trust**.</span><span class="sxs-lookup"><span data-stu-id="c43ce-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="c43ce-120">Așa cum se descrie în documentele noastre, dispozitivele hibrid Azure AD-joint nu pot funcționa în acest caz.</span><span class="sxs-lookup"><span data-stu-id="c43ce-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="c43ce-121">Vă rugăm să lucrați cu furnizorul de identitate pentru asistență.</span><span class="sxs-lookup"><span data-stu-id="c43ce-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="c43ce-122">**Utilizatorii folosesc browserul Chrome fără ca conturile Windows 10** sau **extensia Office Chrome să utilizeze în mod automat PRT-ul pe dispozitivele pe** care le-ați alăturat sau hibrid-s-a alăturat: aceasta conduce la eșecul oricăror politici de acces condiționat bazate pe dispozitiv, cu mesajul de eroare "dispozitiv neînregistrat" afișat.</span><span class="sxs-lookup"><span data-stu-id="c43ce-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="c43ce-123">Pentru a utiliza corect browserul Chrome, trebuie să instalați "conturile Windows 10" sau "extinderea Office la browserul Chrome al utilizatorilor" prin SCCM sau Intune.</span><span class="sxs-lookup"><span data-stu-id="c43ce-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="c43ce-124">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="c43ce-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="c43ce-125">Dacă nu este posibil să apăsați extensia de la distanță, notificați-i pe utilizatori să instaleze manual una dintre extensiile de mai sus pentru a accesa aplicațiile din spatele accesului condiționat bazat pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="c43ce-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="c43ce-126">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="c43ce-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="c43ce-127">**Dispozitivul a fost corect AZURE AD Azure s-a alăturat, dar a fost șters sau dezactivat din greșeală, fie din cauza modificărilor de sincronizare din AZURE AD Connect, fie din portalul Azure**: dacă se întâmplă acest lucru, obiectul dispozitiv nu mai este recunoscut ca dispozitiv complet asociat, chiar dacă starea "AzureAdJoined" și "PRT" se afișează ca valid pe dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="c43ce-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="c43ce-128">Pentru a remedia această problemă, rulează `dsregcmd/leave` pe dispozitivele afectate și permiteți-le să se reasocieze la AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="c43ce-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="c43ce-129">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="c43ce-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="c43ce-130">Dacă dispozitivele dumneavoastră sunt în Windows 10, 1809 Update, cu VPN/Cloud proxy și Vedeți problemele cu starea "AzureAdPrt" sau cu orice aplicație cu SSO problemă (Outlook nu se conectează la cutia poștală, chiar dacă ați avut PRT), asigurați-vă că aveți acest patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) sau actualizarea cumulativă din aprilie [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) pentru a împiedica erorile PRT pe acele mașini.</span><span class="sxs-lookup"><span data-stu-id="c43ce-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















