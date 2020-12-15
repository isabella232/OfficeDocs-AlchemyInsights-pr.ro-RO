---
title: Dispozitiv în stare în așteptare
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679989"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="f4701-102">Dispozitiv în stare în așteptare</span><span class="sxs-lookup"><span data-stu-id="f4701-102">Device in pending state</span></span>

<span data-ttu-id="f4701-103">**Cerințe preliminare**</span><span class="sxs-lookup"><span data-stu-id="f4701-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="f4701-104">Dacă configurați înregistrările dispozitivelor pentru prima dată, asigurați-vă că ați revizuit [Introducere în gestionarea dispozitivelor în Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) care vă va ghida despre cum să obțineți dispozitive sub controlul Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4701-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="f4701-105">Dacă înregistrați dispozitivele în Azure AD direct și le înscrieți în Intune, va trebui să vă asigurați că ați [configurat Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) și că [licența](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) a fost implementată mai întâi.</span><span class="sxs-lookup"><span data-stu-id="f4701-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="f4701-106">Asigurați-vă că sunteți autorizat să efectuați operațiuni în Azure AD și AD local.</span><span class="sxs-lookup"><span data-stu-id="f4701-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="f4701-107">Doar un administrator global din Azure AD poate gestiona setările pentru înregistrările dispozitivelor.</span><span class="sxs-lookup"><span data-stu-id="f4701-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="f4701-108">În plus, dacă configurați înregistrări automate în Active Directory local, va trebui să fiți administrator al Active Directory și AD FS (dacă este cazul).</span><span class="sxs-lookup"><span data-stu-id="f4701-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="f4701-109">Procesul de înregistrare a asocierii hibride Azure AD necesită ca dispozitivele să fie în rețeaua corporativă.</span><span class="sxs-lookup"><span data-stu-id="f4701-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="f4701-110">De asemenea, funcționează prin VPN, dar există câteva limitări pentru aceasta.</span><span class="sxs-lookup"><span data-stu-id="f4701-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="f4701-111">Am auzit clienți care au nevoie de asistență pentru depanarea procesului de înregistrare hibrid Azure AD Join-up, sub circumstanțe de lucru la distanță.</span><span class="sxs-lookup"><span data-stu-id="f4701-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="f4701-112">**Mediu de autentificare în cloud (utilizând Azure AD password hash-sincronizare sau autentificare directă)**</span><span class="sxs-lookup"><span data-stu-id="f4701-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="f4701-113">Acest flux de înregistrare este, de asemenea, cunoscut sub numele de "asociere la sincronizare".</span><span class="sxs-lookup"><span data-stu-id="f4701-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="f4701-114">Iată o defalcare a ceea ce se întâmplă în timpul procesului de înregistrare:</span><span class="sxs-lookup"><span data-stu-id="f4701-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="f4701-115">Windows 10 descoperă înregistrarea punctului de conexiune la serviciu (SCP) atunci când utilizatorul se conectează la dispozitiv.</span><span class="sxs-lookup"><span data-stu-id="f4701-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="f4701-116">Dispozitivul încearcă mai întâi să regăsească informațiile despre entitatea găzduită din partea client SCP în registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="f4701-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="f4701-117">Pentru mai multe informații, consultați [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="f4701-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="f4701-118">Dacă nu reușește, dispozitivul comunică cu Active Directory local pentru a obține informații despre entitatea găzduită de la SCP.</span><span class="sxs-lookup"><span data-stu-id="f4701-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="f4701-119">Pentru a verifica SCP, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="f4701-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="f4701-120">Vă recomandăm să activați SCP în Active Directory și doar să utilizați SCP client-side pentru validare inițială.</span><span class="sxs-lookup"><span data-stu-id="f4701-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="f4701-121">Windows 10 încearcă să comunice cu Azure AD sub contextul sistemului, pentru a se autentifica împotriva Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4701-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="f4701-122">Puteți verifica dacă dispozitivul poate accesa resursele Microsoft sub contul sistemului, utilizând [scriptul de conectivitate pentru înregistrarea dispozitivelor de testare](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="f4701-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="f4701-123">Windows 10 generează certificat cu semnătură automată și îl stochează sub obiectul computer în Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="f4701-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="f4701-124">Acest lucru necesită o linie de vedere la controlerul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="f4701-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="f4701-125">Obiectul dispozitiv care are certificat este sincronizat cu Azure AD prin Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f4701-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="f4701-126">Ciclul de sincronizare este la fiecare 30 de minute în mod implicit, dar depinde de configurarea Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f4701-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="f4701-127">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="f4701-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="f4701-128">În această etapă, ar trebui să puteți vedea dispozitivul subiect în starea "în **așteptare**" sub Blade Device din Azure portal.</span><span class="sxs-lookup"><span data-stu-id="f4701-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="f4701-129">La următorul utilizator de conectare la Windows 10, înregistrarea va fi finalizată.</span><span class="sxs-lookup"><span data-stu-id="f4701-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f4701-130">Dacă vă aflați pe VPN și logoff/login termină conectivitatea domeniului, puteți să declanșați manual înregistrarea.</span><span class="sxs-lookup"><span data-stu-id="f4701-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="f4701-131">Pentru a face acest lucru:</span><span class="sxs-lookup"><span data-stu-id="f4701-131">To do that:</span></span>
    >
    > <span data-ttu-id="f4701-132">Emiteți o `dsregcmd /join` Solicitare locală în administrare sau la distanță prin PSExec pe PC.</span><span class="sxs-lookup"><span data-stu-id="f4701-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="f4701-133">De exemplu: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="f4701-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="f4701-134">Pentru probleme comune cu înregistrarea dispozitivelor Azure Active Directory, consultați [întrebări frecvente despre dispozitive](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="f4701-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
