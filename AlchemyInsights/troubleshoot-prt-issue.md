---
title: Depanarea problemei PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ro-RO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573724"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="285e6-102">Depanarea problemei PRT</span><span class="sxs-lookup"><span data-stu-id="285e6-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="285e6-103">Pentru ca orice dispozitiv să termine să se autentifice, acesta trebuie să fie înregistrat complet și în stare bună și să poată obține un token de reîmprospătare principală (PRT).</span><span class="sxs-lookup"><span data-stu-id="285e6-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="285e6-104">Procesul de înregistrare a asocierii hibride Azure AD necesită ca dispozitivele să fie într-o rețea corporativă.</span><span class="sxs-lookup"><span data-stu-id="285e6-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="285e6-105">De asemenea, funcționează prin VPN, dar există câteva limitări pentru aceasta.</span><span class="sxs-lookup"><span data-stu-id="285e6-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="285e6-106">Am auzit clienți care au nevoie de asistență cu depanarea procesului de înregistrare hibrid Azure AD Join-up în circumstanțe de la locul de muncă.</span><span class="sxs-lookup"><span data-stu-id="285e6-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="285e6-107">Iată o defalcare a ceea ce se întâmplă "sub capota" în timpul procesului de înregistrare.</span><span class="sxs-lookup"><span data-stu-id="285e6-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="285e6-108">**Mediu de autentificare în cloud (utilizând Azure AD password hash-sincronizare sau autentificare directă)**</span><span class="sxs-lookup"><span data-stu-id="285e6-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="285e6-109">Acest flux de înregistrare este, de asemenea, cunoscut sub numele de "asociere la sincronizare".</span><span class="sxs-lookup"><span data-stu-id="285e6-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="285e6-110">Windows 10 descoperă o înregistrare SCP la conectarea la utilizator a dispozitivului.</span><span class="sxs-lookup"><span data-stu-id="285e6-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="285e6-111">Dispozitivul încearcă mai întâi să regăsească informațiile despre entitatea găzduită din partea client SCP în registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="285e6-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="285e6-112">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="285e6-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="285e6-113">Dacă nu reușește, dispozitivul comunică cu Active Directory local (AD) pentru a obține informații despre entitatea găzduită de la punctul de conexiune la serviciu (SCP).</span><span class="sxs-lookup"><span data-stu-id="285e6-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="285e6-114">Pentru a verifica SCP, vă rugăm să consultați acest [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="285e6-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="285e6-115">Vă recomandăm să activați SCP în reclamă și să utilizați doar clientul-Side SCP pentru validare inițială.</span><span class="sxs-lookup"><span data-stu-id="285e6-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="285e6-116">Windows 10 încearcă să comunice cu Azure AD sub contextul sistemului, pentru a se autentifica împotriva Azure AD.</span><span class="sxs-lookup"><span data-stu-id="285e6-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="285e6-117">Puteți verifica dacă dispozitivul poate accesa resursele Microsoft sub contul sistemului, utilizând scriptul de conectivitate pentru înregistrarea dispozitivelor de testare.</span><span class="sxs-lookup"><span data-stu-id="285e6-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="285e6-118">Windows 10 generează un certificat cu semnătură automată și îl stochează sub obiectul computer din reclama locală.</span><span class="sxs-lookup"><span data-stu-id="285e6-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="285e6-119">Acest lucru necesită o linie de vedere la controlerul de domeniu.</span><span class="sxs-lookup"><span data-stu-id="285e6-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="285e6-120">Un obiect dispozitiv care are un certificat este sincronizat cu Azure AD prin Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="285e6-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="285e6-121">Ciclul de sincronizare este la fiecare 30 de minute în mod implicit, dar depinde de configurarea Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="285e6-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="285e6-122">Pentru mai multe informații, consultați acest [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="285e6-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="285e6-123">În această etapă, ar trebui să puteți vedea dispozitivul subiect în starea "în așteptare" sub Blade Device din Azure portal.</span><span class="sxs-lookup"><span data-stu-id="285e6-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="285e6-124">La următorul utilizator de conectare la Windows 10, înregistrarea va fi finalizată.</span><span class="sxs-lookup"><span data-stu-id="285e6-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="285e6-125">Dacă vă deconectați de la VPN și un proces de conectare la logoff termină conectivitatea domeniului, puteți să declanșați manual înregistrarea:</span><span class="sxs-lookup"><span data-stu-id="285e6-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="285e6-126">Emiteți un dsregcmd/Join local pe un prompt de administrator sau la distanță prin PSExec pe PC.</span><span class="sxs-lookup"><span data-stu-id="285e6-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="285e6-127">De exemplu, PsExec-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="285e6-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="285e6-128">Pentru mai multe detalii despre problemele de asociere hibrid, consultați [Depanarea problemei dispozitivelor](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="285e6-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
